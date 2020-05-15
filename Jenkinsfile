pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/innomatics321/DevOps-UIUX.git', branch: 'master')
      }
    }

  }
  environment {
    dev = 'develop'
  }
}