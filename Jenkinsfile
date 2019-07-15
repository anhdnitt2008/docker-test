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
                sh 'npm start' 
            }
        }
    }
}
