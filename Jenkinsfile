pipeline {
    agent {
        label 'agent'
    }
    tools {
        terraform 'Terraform'
    }

    stages {
        stage('Get Code') {
            steps {
                checkout scm
            }
        }  
    }
}