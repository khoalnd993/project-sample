pipeline {
    agent none
    stages {
        stage('Get code') {
            agent { docker 'gcc:latest' }
            steps {
                sh 'make clean-all'
            }
        }
        stage('Clean environment') {
            steps {
                sh 'make clean-obj'
            }
        }
    }
}
