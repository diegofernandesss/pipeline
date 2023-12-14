pipeline {
    agent { docker { image 'python:3.10' } }
    stages {
        stage('build') {
            steps {
                script {
                    sh 'pip install --user flask'
                    sh 'chmod -R 777 /.local'
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
