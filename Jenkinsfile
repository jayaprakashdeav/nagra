pipeline {
  agent any
  stages {
    stage('UT/CIT') {
      steps {
        echo 'UT/CIT'
      }
    }
    stage('Build') {
      steps {
        echo 'Build'
      }
    }
    stage('ST') {
      steps {
        echo 'ST'
      }
    }
    stage('Report') {
      parallel {
        stage('Report') {
          steps {
            echo 'Report'
          }
        }
        stage('Regression') {
          steps {
            echo 'Regression'
          }
        }
      }
    }
  }
}