pipeline {
    agent none
    agent {
        docker {
            image 'python:3.8-slim'
}
    }

    stages {
        stage('Check Python Version') {
            steps {
                echo 'Vérification de la version de Python...'
                sh 'python --version'
            }
        }

        stage('Execute Python Script') {
            steps {
                echo 'Exécution du script random_grade.py...'
                sh 'python random_grade.py'
            }
        }
    }
}
