pipeline {
    agent any
    
    stages {

        stage('install Requirementse') {
            steps
            {
                sh"pip3 install requirements.txt"
            }
            }
        stage('build project'){
            steps
            {
                sh"python app.py"
            }
        }
        }
    }

