pipeline {
    agent any
    tools {
        maven 'Maven3' // This name must match the Name in Step 3 
        jdk 'JDK17'    // This name must match the Name in Step 2 
    }
    stages {
        stage('Checkout') {
            steps {
                // Ensure this URL is your specific repository
                git 'https://github.com/Anikesh0001/demo-app-.git' [cite: 160]
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile' [cite: 165]
            }
        }
        // ... include Test and Package stages as well [cite: 168, 173]
    }
}
