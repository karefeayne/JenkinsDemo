pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "echo Building Stage1"
                sh "cd frontend && npm install && npm run build"
            }
            
        }

        stage('Deploy Frontend'){
            steps{
                script{
                      withAWS(region: 'us-east-1', credentials: 'AWS_CREDENTIALS'){
                        sh "aws s3 sync frontend/dist s3://boardgame-inventory-management" 
                        }   
                }
            }
        }
    }
}
