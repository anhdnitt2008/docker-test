pipeline {
    agent {
        docker {
            image 'docker-test-1:latest' 
            args '-p 3001:9001' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'docker run -it -p 3001:9001 docker-test-1:latest' 
            }
        }
    }
}
