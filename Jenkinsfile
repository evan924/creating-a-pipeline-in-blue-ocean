pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        powershell(script: 'sudo apt-get install npm', returnStatus: true, returnStdout: true)
      }
    }
  }
}