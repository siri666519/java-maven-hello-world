pipeline {
    agent any

    tools {
        maven 'MAVEN_HOME'  // Make sure you define this Maven tool in Jenkins Global Tool Config
        jdk 'JAVA_HOME'     // Also define JDK in Jenkins tools
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


