pipeline {
    agent any 
    stages {
        stage('Deploy') {
            steps {
                git 'https://github.com/chuoi2cu/auto-deploy-server.git'
            }
        }
        stage('SSH server'){
            steps{
                sshagent (['deploy-dev']) {
                    sh 'ssh -o StrictHostKeyChecking=no -l root 159.89.224.222 touch test.txt'
                }
            }
       }
    }
}
