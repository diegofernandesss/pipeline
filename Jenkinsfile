pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                script {
                    sh 'chmod 777 /.local'
                    sh 'pip install --user flask'
                }
            }
        }
        stage('test') {
            steps {
                sh 'python test.py'
            }
        }
    }
}
