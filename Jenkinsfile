pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment { 
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh '''
                    chmod +x './jenkins/scripts/test.sh'
                    './jenkins/scripts/test.sh'
                   '''
            }
        }
        stage('Deliver') { 
            steps {
                sh '''
                    chmod +x './jenkins/scripts/deliver.sh'
                   './jenkins/scripts/deliver.sh' 
                '''
                input message: '¿Terminaste de usar el sitio Web? (Da click en "Proceed" para continuar)' 
                sh '''
                   chmod +x './jenkins/scripts/kill.sh'
                   './jenkins/scripts/kill.sh'
                   '''
            }
        }
    }
}
