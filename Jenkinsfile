pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'bash -c pip install flask'
            }
        }
        stage('test') {
            steps {
                sh 'bash -c python test.py'
            }
        }
    }
}
