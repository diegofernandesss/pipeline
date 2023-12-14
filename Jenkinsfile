pipeline {
    agent { docker { image 'python:3.7.2' } }
    environment {
        ATIVACAO_VENV = 'env/bin/activate'
    }
    stages {
        stage('build') {
            steps {
                sh 'python -m venv env'
                sh 'ash -c "source $ATIVACAO_VENV && pip install flask"'
            }
        }
        stage('test') {
            steps {
                sh 'ash -c "source $ATIVACAO_VENV && python test.py"'
            }
        }
    }
}
