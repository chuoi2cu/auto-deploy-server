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
                sshagent(['ssh-remote-root']) {
                    sh 'ssh -o StrictHostKeyChecking=no -l root 159.89.224.222 uname -a'
                }
            }
       }
    }
}
