pipeline {
    agent any

    tools {
        maven 'MAVEN_HOME'
    }

    stages {
        stage('Build') {
            steps {
                // Execute build commands or scripts
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Execute test commands or scripts
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                // Execute packaging commands or scripts
                bat 'mvn package'
            }
        }

        stage('Deploy') {
            steps {
                // Execute deployment commands or scripts
                bat 'mvn deploy'
            }
        }
    }
}
