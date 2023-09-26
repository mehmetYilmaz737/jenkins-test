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
                sh 'docker ps -a'
            }
        }
    }
}
