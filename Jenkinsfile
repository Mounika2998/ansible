pipeline {
    agent { label 'ws' }
    environment { 
        SSH_CREDENTIALS = credentials('SSH_CRED') 
    }    
    stages {
    
    stage('Promotion To Prod Branch') {       // This stage will run only against the main branch
            steps {
                sh "env"
                sh "I am samplerun branch"
                sh "echo main - PROMOTING To PROD"
            }
        }
    }
}
