pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        git(url: 'https://github.com/innomatics321/Amazon', branch: 'master')
      }
    }

    stage('validate') {
      steps {
        git(url: 'https://github.com/innomatics321/Amazon.git', branch: 'master')
      }
    }

  }
}