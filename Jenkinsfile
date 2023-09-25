pipeline {
    agent {
        docker { image 'dind:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'docker ps -a'
            }
        }
    }
}
