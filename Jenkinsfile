pipeline {
    agent { docker { dockerfile true } }
    // agent any
    stages {
        stage('test') {
            steps {
                //sh 'PYTHONPATH=. pytest'
                sh 'python -m pip install --no-cache-dir pytest'
                sh 'python -m pytest tests'
            }
        }
    }
}
