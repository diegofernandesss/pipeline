
pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'python -m venv env'
                sh '''source ./env/bin/activate; 
                      sh -c "pip install flask"'''
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
