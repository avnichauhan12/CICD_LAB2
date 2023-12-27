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
                echo 'build'
            }
        }
        
        stage('Test') {
            steps {
            
                echo 'No tests defined for HTML content'
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
