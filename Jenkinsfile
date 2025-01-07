pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'pytest tests/'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-app .'
            }
        }
    }
}



