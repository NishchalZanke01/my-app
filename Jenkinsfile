pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building the application...'
                bat '"C:\\Users\\nishc\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run') {
            steps {
                bat '"C:\\Users\\nishc\\AppData\\Local\\Programs\\Python\\Python311\\python.exe" app.py'
            }
        }
    }
}
