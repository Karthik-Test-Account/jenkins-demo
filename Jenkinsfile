pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Use 'git' step to check out from a specific repository and branch
                git url: 'https://github.com/Karthik-Test-Account/jenkins-demo.git', branch: 'main'
            }
        }

        stage('Run Python Scripts') {
            parallel {
                stage('Run script1.py') {
                    steps {
                        bat 'python hello.py'  // Use 'bat' for Windows
                    }
                }
                stage('Run script2.py') {
                    steps {
                        bat 'python pip.py'  // Use 'bat' for Windows
                    }
                }
                stage('Run script3.py') {
                    steps {
                        bat 'python sample.py'  // Use 'bat' for Windows
                    }
                }
            }
        }
    }
}
