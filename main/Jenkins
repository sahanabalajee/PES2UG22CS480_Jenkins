pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o YOUR_SRN-1 main.cpp'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES2UG22CS480-1'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
