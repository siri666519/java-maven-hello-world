pipeline {
    agent any

    tools {
        maven 'Maven 3.8.1'     // This matches your configured tool name
        jdk 'JDK 11'            // Make sure this is the correct JDK name in your Jenkins too
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/siri666519/java-maven-hello-world.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}



