pipeline {
    agent any
    
    stages {

        stage('install Requirementse') {
            steps
            {
                sh"pip install requirements.txt"
            }
            }
        stage('build project'){
            steps
            {
                sh"python3 app.py"
            }
        }
        }
    }

