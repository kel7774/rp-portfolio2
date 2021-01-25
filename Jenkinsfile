pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Build') {
            steps {
                sh 'python3 --version'
                sh 'pip install django'
            }
        }
        stage('Test'){
            steps{
              sh 'python manage.py runserver'
            }
        }
    }
}
