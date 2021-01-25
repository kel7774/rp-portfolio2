pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('Build') {
            steps {
                sh 'python3 --version'
            }
        }
        stage('Test'){
            steps{
              sh 'python3 manage.py runserver'
            }
        }
    }
}
