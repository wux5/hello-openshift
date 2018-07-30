pipeline {
  agent {
    docker {
      image 'node:10-alpine'
      args '-v ${WORKSPACE}:/hello-openshift'
    }

  }
  stages {
    stage('test') {
      steps {
        sh '''node --version;
cd /hello-openshift;
ls -l;
#npm install && npm test'''
      }
    }
  }
}