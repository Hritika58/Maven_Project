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
    }
}
