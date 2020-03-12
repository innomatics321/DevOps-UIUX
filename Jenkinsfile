pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            git(url: 'https://github.com/innomatics321/DevOps-UIUX.git', branch: 'master')
            echo 'This is a minimal pipeline'
            bat 'echo %Name%'
          }
        }

        stage('build 2') {
          steps {
            bat 'echo Build2'
          }
        }

      }
    }

    stage('test') {
      steps {
        bat 'echo test'
      }
    }

  }
}