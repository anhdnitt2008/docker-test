pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'docker build --rm -f "Dockerfile" -t docker-test-3:latest .' 
            }
        }
        stage('Deploy') { 
            steps {
                sh 'docker run -it -p 3003:9001 docker-test-3' 
            }
        }
    }
}