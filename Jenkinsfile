pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'echo "Build"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Test"'
            }
        }
        stage('Deliver for development') {
            when {
                branch 'development' 
            }
            steps {
                sh 'echo "development"'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'  
            }
            steps {
                sh 'echo "production"'
            }
        }
    }
}
