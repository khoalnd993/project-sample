pipeline {
    agent any
    stages {
        stage('Get code') {
            steps {
                sh 'git clone https://github.com/khoalnd993/project-sample.git'
            }
        }
        stage('Example Test') {
            steps {
                echo 'Hello, JDK'
            }
        }
    }
}
