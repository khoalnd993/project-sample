pipeline {
    agent { docker 'gcc:latest' }
    stages {
        stage('Get code') {
            steps {
                sh 'git clone https://github.com/khoalnd993/project-sample.git'
            }
        }
        stage('Clean environment') {
            steps {
                sh 'Make clean'
            }
        }
    }
}
