 pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'pytest'
            }
        }

        stage('Build') {
            steps {
                bat 'mkdir build'
                bat 'copy app.py build\\app.py'
                bat 'copy requirements.txt build\\requirements.txt'
            }
        }
    }
}