pipeline {
    agent any
    tools {
        maven 'Maven3' // Must match the Name in Global Tool Configuration
        jdk 'JDK17'    // Must match the Name in Global Tool Configuration
    }
    stages {
        stage('Checkout') {
            steps {
                // Ensure this matches your specific repository
                git 'https://github.com/Anikesh0001/demo-app-.git' [cite: 160]
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile' [cite: 165]
            }
        }
        // ... rest of your stages [cite: 168, 173]
    }
}
