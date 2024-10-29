pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Karthik-Test-Account/jenkins-demo.git', branch: 'main'
            }
        }
        stage('Build Job1') {
            steps {
                sh 'python3 hello.py'
            }
        }
        stage('Build Job2') {
            steps {
                sh 'python3 pip.py'
            }
        }
        stage('Build Job3') {
            steps {
                sh 'python3 sample.py'
            }
        }
    }
}
