pipeline {
    agent { docker { image 'python:3.9.4' } }
    stages {
        stage('build') {
            steps {
                sh 'pip install --user -r requirements.txt'
            }
        }
        stage('test') {
            steps {
                sh 'python test.py"'
            }
        }
    }
}
