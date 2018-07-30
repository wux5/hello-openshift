pipeline {
  agent {
    docker {
      image 'node:10-alpine'
      args '-v /var/jenkins_home/workspace/hello-openshift_master-OTCQ7HRG5LFS5XX2GBATFTQSZRZU6DNQVVVGXX5K2GHSATO4JC6Q:/hello-openshift'
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