pipeline {
    agent any

    tools {
        maven 'Maven 3.8.1'     // Must match Jenkins tool name
        jdk 'JDK 11'            // Must match Jenkins tool name
    }

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/siri666519/java-maven-hello-world.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}




