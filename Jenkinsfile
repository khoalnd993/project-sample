pipeline {
    agent none
    stages {
        stage('Get code') {
            agent { docker 'gcc:latest' }
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
