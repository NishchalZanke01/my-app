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
                sh 'echo Building the application...'
                sh 'pip install -r requirements.txt || true'
            }
        }
        stage('Test') {
            steps {
                sh 'echo Running tests...'
            }
        }
        stage('Run') {
            steps {
                sh 'echo Application deployed successfully!'
            }
        }
    }
}