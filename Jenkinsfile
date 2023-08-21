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
        stage('Clean running containers') {
            steps {
                sh "docker rm -f frontend backend"
            }
        }
    }
}