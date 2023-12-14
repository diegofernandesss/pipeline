pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'virtualenv venv'
                sh 'bash -c ". venv/bin/activate && pip install flask"'
            }
        }
        stage('test') {
            steps {
                sh 'bash -c ". venv/bin/activate && python test.py"'
            }
        }
    }
}
