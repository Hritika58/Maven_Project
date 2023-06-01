pipeline {
    agent any

    tools {
        maven 'MAVEN_HOME'
    }

    stages {
        stage('Build') {
            steps {
                // Execute build commands or scripts
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'c6c7c9de-81f3-4852-b561-5dfe01b14c59', url: 'https://github.com/Hritika58/Maven_Project.git']])
                sh "mvn clean compile"
            }
        }

        stage('Test') {
            steps {
                // Execute test commands or scripts
                sh "mvn test"
            }
        }

        stage('Package') {
            steps {
                // Execute packaging commands or scripts
                sh "mvn package"
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
