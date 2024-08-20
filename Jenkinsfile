pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "echo Building Stage1"
            }
        }

        stage('Test') {
            steps {
                sh "echo Testing Stage2"
            }
        }

        stage('testGitWebhook') {
            steps {
                sh "echo TIt Works"
            }
        }

        stage('Deploy') {
            steps {
                sh "echo Deploying Stage3"
            }
        }
    }
}
