pipeline {
    agent { docker { image 'python:3.7.2', args:'-u root:root' } }
    stages {
        stage('build') {
            steps {
                sh 'pip install flask"'
            }
        }
        stage('test') {
            steps {
                sh 'python test.py"'
            }
        }
    }
}
