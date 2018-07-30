pipeline {
  agent {
    docker {
      image 'node:10-alpine'
    }

  }
  stages {
    stage('test') {
      agent {
        docker {
          image 'node:10-alpine'
        }

      }
      steps {
        sh 'echo "Hello docker...."'
      }
    }
  }
}