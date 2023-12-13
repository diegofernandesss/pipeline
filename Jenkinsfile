pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'sh -c pip install flask'
            }
        }
        stage('test') {
            steps {
                sh 'sh -c python test.py'
            }
        }
    }
}
