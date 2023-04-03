pipeline {
    agent { label 'ws' }
    environment { 
        SSH_CREDENTIALS = credentials('SSH_CRED') 
    }    
    stages {
        
        stage('Performing Lint Check') {
            steps {
                sh "env"
                sh "echo This step should run against non-main branches only"
                sh "echo PERFORMING LINT CHECKSS"
            }
        }

    }


}