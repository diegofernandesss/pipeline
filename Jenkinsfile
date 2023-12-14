
pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python -m venv env'
                sh '.env/bin/activate; pip install flask'
            }
        }
        stage('test') {
            steps {
                sh '''
                . env/bin/activate
                python test.py
                '''
            }
        }
    }
}
