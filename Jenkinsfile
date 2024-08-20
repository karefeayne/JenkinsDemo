pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "echo Building Stage1"
                sh "cd frontend && npm install && run build"
            }
        }
    }
}
