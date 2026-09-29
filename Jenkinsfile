pipeline {
    agent any

    stages {
        stage('Create Virtual Environment') {
            steps {
                bat '"C:\\Users\\NASHATH V N\\AppData\\Local\\Python\\bin\\python.exe" -m venv venv'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'venv\\Scripts\\python.exe -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'venv\\Scripts\\python.exe -m pytest'
            }
        }
    }
}