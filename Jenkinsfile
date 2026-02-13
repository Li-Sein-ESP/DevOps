pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Li-Sein-ESP/DevOps.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package -DskipTests'
            }
        }
    }
}
