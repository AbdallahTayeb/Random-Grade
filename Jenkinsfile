pipeline {
    agent any

    stages {
        stage('Check Python Version') {
            steps {
                echo 'Checking Python version...'
                sh 'python --version || python3 --version'
            }
        }

        stage('Run Python Script') {
            steps {
                echo 'Running app.py...'
                sh 'python app.py || python3 app.py'
            }
        }
    }
}
