pipeline {

    stages {

        stage('install Requirements') {
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
}
