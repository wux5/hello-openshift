pipeline {
  agent {
    docker {
      image 'node:10-alpine'
      args '-v ./:/hello-openshift'
    }

  }
  stages {
    stage('test') {
      steps {
        sh '''node --version;
npm install && npm test'''
      }
    }
  }
}