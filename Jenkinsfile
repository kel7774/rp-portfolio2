pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Build') {
            steps {
                sh 'python --version'
                sh 'sudo pip install django-jenkins'
            }
        }
        stage('Test'){
            steps{
              sh 'python manage.py runserver'
            }
        }
    }
}
