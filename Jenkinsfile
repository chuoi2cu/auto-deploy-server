pipeline {
    agent any 

    stages {
        stage ('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://<token>@github.com/username/repoName.git'
            }
        },
        stage('Deploy') {
            steps {
                git 'https://github.com/chuoi2cu/auto-deploy-server.git'
            }
        }
        
    }
}