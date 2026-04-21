pipeline {
    agent any
    
    tools {
        maven 'Maven3'
        jdk 'JDK17'
    }
    
    stages {
        stage('Checkout') {
            steps {
                // Explicitly defining the 'main' branch
                git branch: 'main', url: 'https://github.com/Anikesh0001/demo-app-.git'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
