pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Vallabh04022006/assessment-7.2.git'
            }
        }

        stage('Generate Report') {
            steps {
                bat 'C:\Users\Vallabh\AppData\Local\Python\bin\python.exe'
            }
        }

        stage('Archive Report') {
            steps {
                archiveArtifacts artifacts: 'report.txt', fingerprint: true
            }
        }
    }
}
