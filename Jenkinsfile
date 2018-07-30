pipeline {
  agent {
    docker {
      image 'node:10-alpine'
    }

  }
  stages {
    stage('kick off') {
      steps {
        sh '''echo "Let\'s start";
docker version'''
      }
    }
    stage('build') {
      steps {
        sh 'npm install'
      }
    }
    stage('test') {
      steps {
        sh 'npm test'
      }
    }
    stage('notify') {
      steps {
        sh 'echo "done. good job"'
      }
    }
  }
}