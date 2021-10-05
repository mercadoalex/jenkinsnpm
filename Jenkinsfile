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
        echo 'Montamos el socket'
        sh 'docker run -v /var/run/docker.sock:/var/run/docker.sock            -ti docker'
        echo 'Construimos la app'
        sh '/usr/bin/npm install'
      }
    }

  }
}