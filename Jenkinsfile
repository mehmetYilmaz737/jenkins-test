pipeline {
    agent {
        docker { 
            image 'docker:dind'
            args '-v /var/run/docker.sock:/var/run/docker.sock -u root'
        }
    }
    stages {
        stage('Test') {
            steps {
                sh '''
                apk update
                apk add jq
                apk add --no-cache aws-cli
                '''
                
            }
        }
    }
}
