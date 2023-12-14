pipeline {
    agent { docker { image 'python:3.7.2' } }
    environment {
        ATIVACAO_VENV = '. venv/bin/activate'
    }
    stages {
        stage('build') {
            steps {
                sh 'python -m venv venv'
                sh '$ATIVACAO_VENV && pip install --upgrade pip && pip install flask'
            }
        }
        stage('test') {
            steps {
                sh 'bash -c "$ATIVACAO_VENV && python test.py"'
            }
        }
    }
}
