pipeline {
  agent {
    node {
      label 'agent01'
    }

  }
  stages {
    stage('Source') {
      steps {
        git(url: 'https://github.com/goormbee-tech/simpleHTTP.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        tool 'gradle'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "Deploy Success"'
      }
    }

  }
}