pipeline {
  agent {
    docker {
      image 'node:10-alpine'
    }

  }
  stages {
    stage('test') {
      steps {
        sh 'docker version'
      }
    }
  }
}