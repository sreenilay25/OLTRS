pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Success') {
            steps {
                echo 'Maven build completed successfully!'
            }
        }
    }
}
