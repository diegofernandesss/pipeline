pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'sudo pip install flask --user'
            }
        }
        stage('test') {
            steps {
                sh 'python test.py'
            }
        }
    }
}
