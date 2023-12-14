pipeline {
    agent { docker { image 'python:3.10' } }
    stages {
        stage('build') {
            steps {
                sh 'python -m pip install flask'
            }
        }
        stage('test') {
            steps {
                sh 'python test.py'
            }
        }
    }
}
