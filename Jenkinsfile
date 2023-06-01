pipeline {
    agent any
    
    environment {
        MVN_HOME = tool 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                // Execute build commands or scripts
                sh "${MVN_HOME}/bin/mvn clean compile"
            }
        }

        stage('Test') {
            steps {
                // Execute test commands or scripts
                sh "${MVN_HOME}/bin/mvn test"
            }
        }

        stage('Package') {
            steps {
                // Execute packaging commands or scripts
                sh "${MVN_HOME}/bin/mvn package"
            }
        }

        stage('Deploy') {
            steps {
                // Execute deployment commands or scripts
                sh '${MVN_HOME}/bin/mvn deploy'
            }
        }
    }
}
