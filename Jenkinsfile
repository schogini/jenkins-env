pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Building1234.."'
        sleep 10
      }
    }
    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            sh 'echo "Test1"'
          }
        }
        stage('Test2') {
          steps {
            sh 'echo "Test2.."'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploy.."'
      }
    }
  }
}
