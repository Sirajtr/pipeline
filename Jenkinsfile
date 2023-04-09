pipeline {
    
    agent any 
    
    environment {
        IMAGE_TAG = "${BUILD_NUMBER}"
    }
    
    stages {
        
        stage('Checkout'){
           steps {
            git 'https://github.com/Sirajtr/pipeline.git'
           }
        
    
    
    stage('Build Docker'){
            steps{
                script{
                    sh '''
                    echo 'Buid Docker Image'
                    docker build -t sirajtr/pipeline:${BUILD_NUMBER} .
                    '''
                }
            }
        }
    }
    }
}       
