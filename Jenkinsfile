pipeline {
    agent any

    stages {      
        stage('Build') {
            steps {
                echo 'Building...'
                // Compile the Java code
                sh 'javac -d target ToUpper.java'
            }
        }       
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Run the Java program with an example argument
                sh 'java -cp target ToUpper "tres tristes tigres"'
            }
        }
    }
}
