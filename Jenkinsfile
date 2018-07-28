pipeline {
  agent any
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