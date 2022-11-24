pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/Ivanmsci/jenkins.git', branch: 'master')
      }
    }

    stage('') {
      steps {
        sh 'ls -la'
      }
    }

  }
}