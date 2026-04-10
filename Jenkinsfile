pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building the application...'
                bat 'py -m pip install -r requirements.txt'
            }
        }

        stage('Run') {
            steps {
                bat 'py app.py'
            }
        }
    }
}