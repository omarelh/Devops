pipeline {
    agent {
        docker { image 'python:3.10' }
    }
    stages {
        stage('Install Dependencies') {
            steps {
                // Install dependencies from requirements.txt
                sh'pip install --upgrade pip'
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                // Run unit tests
                sh 'pytest tests/'
            }
        }
        stage('Build Docker Image') {
            steps {
                // Build a Docker image for the Python app
                sh 'docker build -t your-python-app .'
            }
        }
    }
}


