pipeline {
    agent any

    stages {
       
        stage('Build') {
            steps {
                echo 'Building...'
                // Compile the code using Maven
                bat 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Run tests using Maven
                bat 'mvn test'
            }
        }
        stage('Package') {
            steps {
                echo 'Packaging...'
                // Package the application using Maven
                bat 'mvn package'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Run the Java program with an example argument
                bat 'java -cp \\target your-app-1.0-SNAPSHOT.jar com.apasoft.ToUpper "${Convertir}"'
            }
        }
    }
}
