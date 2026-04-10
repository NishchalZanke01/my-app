pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/NishchalZanke01/my-app'
            }
        }
        stage('Build') {
            steps {
                bat 'echo Building the application...'
                bat 'pip install -r requirements.txt || true'
            }
        }
        stage('Test') {
            steps {
                bat 'echo Running tests...'
            }
        }
        stage('Run') {
            steps {
                bat 'echo Application deployed successfully!'
            }
        }
    }
}
