pipeline {
    stages {
        stage('Build') { 
            steps {
                sh 'docker build --rm -f "Dockerfile" -t docker-test-2:latest .' 
            }
        }
    }
}
