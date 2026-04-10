pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building the application...'
                bat 'python -m pip install -r requirements.txt'
            }
        }

        stage('Run') {
            steps {
                bat 'python app.py'
            }
        }
    }
}
