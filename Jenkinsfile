pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/Ivanmsci/jenkins.git', branch: 'master')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front end test unit') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}