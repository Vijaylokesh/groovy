pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo " hai"'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo " test is triggerd"'
          }
        }
        stage('unit test') {
          steps {
            sh 'echo " unit test is running"'
          }
        }
        stage('integration test') {
          steps {
            sh 'echo " integration test"'
          }
        }
        stage('sanity test') {
          steps {
            sh 'echo " hai sanity"'
          }
        }
      }
    }
    stage('stagging area') {
      steps {
        sh 'echo " hai stagging area"'
      }
    }
    stage('prod') {
      steps {
        sh 'echo " hai prods"'
      }
    }
  }
}
