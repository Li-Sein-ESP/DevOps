pipeline {
    agent any

    tools {
        maven 'M2_HOME'
    }

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/YOUR-REPO-URL.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }

        stage('Run App (optional)') {
            steps {
                sh 'echo "Build completed successfully"'
            }
        }
    }
}
