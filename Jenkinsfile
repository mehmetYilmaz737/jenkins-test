pipeline {
    agent {
        docker { 
            image 'docker:dind'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh '''
                sudo apt update 
                sudo apt upgrade -y
                sudo apt insall curl
                curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
                unzip awscliv2.zip
                sudo ./aws/install
                '''
                
            }
        }
    }
}
