pipeline {
  agent {
    docker {
      image 'node:10-alpine'
      args '-v `pwd`:/hello-openshift'
    }

  }
  stages {
    stage('test') {
      steps {
        sh '''node --version;
cd /hello-openshift;
npm install && npm test'''
      }
    }
  }
}