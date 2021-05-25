pipeline {
    agent { docker 'gcc:latest' }
    stages {
        stage('Get code') {
            steps {
                sh 'make clean-all'
            }
        }
        stage('Clean object') {
            steps {
                sh 'make clean-obj'
            }
        }
        stage('build') {
            steps {
                sh 'make'
            }
        }
    }
    post {
      success {
        echo "SUCCESSFUL"
      }
      failure {
        echo "FAILED"
      }
    }
}
