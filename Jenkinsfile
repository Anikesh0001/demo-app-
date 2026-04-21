pipeline {
    agent any
    
    tools {
        // These must match the names in Global Tool Configuration
        maven 'Maven3'
        jdk 'JDK17'
    }
    
    stages {
        // We skip the manual 'Checkout' stage because Jenkins 
        // does this automatically at the start of the build.

        stage('Build') {
            steps {
                // Compiles the source code [cite: 165]
                sh 'mvn clean compile'
            }
        }
        
        stage('Test') {
            steps {
                // Runs the JUnit tests [cite: 170]
                sh 'mvn test'
            }
        }
        
        stage('Package') {
            steps {
                // Creates the JAR file in the target directory [cite: 176]
                sh 'mvn package'
            }
        }
    }
}
