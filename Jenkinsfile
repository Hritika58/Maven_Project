pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Execute build commands or scripts
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                // Execute test commands or scripts
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                // Execute packaging commands or scripts
                sh 'mvn package'
            }
        }

        stage('Deploy') {
            steps {
                // Execute deployment commands or scripts
                sh 'mvn deploy'
            }
        }
    }
}
