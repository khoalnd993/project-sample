pipeline {
    agent { docker 'gcc:latest' }
    stages {
        stage('Get code') {
            agent { docker 'gcc:latest' }
            steps {
                sh 'git clone https://github.com/khoalnd993/project-sample.git'
            }
        }
        stage('Clean environment') {
            agent { docker 'gcc:latest' }
            steps {
                sh 'Make clean'
            }
        }
    }
}
