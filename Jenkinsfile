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
                 sh "ansible-playbook robot-dryrun.yaml -e COMPONENT=mongodb -e ansible_user=${SSH_CREDENTIALS_USR} -e ansible_password=${SSH_CREDENTIALS_PSW} -e ENV=qa"
                sh "echo PERFORMING LINT CHECKSS"
            }
        }

    }


}