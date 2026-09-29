 pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                bat 'D:\\python jenkins\\venv\\Scripts\\python.exe -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'D:\\python jenkins\\venv\\Scripts\\python.exe -m pytest'
            }
        }
    }
}