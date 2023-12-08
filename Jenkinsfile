pipeline {
    agent python

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
                sh 'python random_grade.py || python3 random_grade.py'
            }
        }
    }
}
