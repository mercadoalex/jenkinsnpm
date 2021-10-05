pipeline {
  agent {
    any {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'Construimos la app'
        sh 'npm install'
      }
    }

  }
}