pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        git(url: 'https://github.com/innomatics321/Amazon', branch: 'master')
      }
    }

    stage('validate') {
      parallel {
        stage('validate') {
          steps {
            git(url: 'https://github.com/innomatics321/Amazon.git', branch: 'master')
          }
        }

        stage('testing') {
          steps {
            git(url: 'https://github.com/innomatics321/DevOps-UIUX.git', branch: 'master')
          }
        }

        stage('package') {
          steps {
            bat 'mvn package'
          }
        }

      }
    }

  }
}