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
        }
    }
}       
