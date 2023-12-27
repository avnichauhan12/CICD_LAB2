pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {                
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                sh 'cp index.html build/' // Copy index.html to a build directory
            }
        }
        
        stage('Test') {
            steps {
            
                sh 'echo "No tests defined for HTML content"'
            }
        }
        
    }
    
    post {
        success {
            echo 'Pipeline succeeded! Project built and deployed.'
        }
        failure {
            echo 'Pipeline failed! Check logs for details.'
        }
    }
}
