
pipeline {
    agent any

    tools {
        maven 'maven'
    }

    stages {
        stage('Checkout') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/santhosh8328/Train-Ticket-Reservation-System.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Confirmation') {
            steps {
                echo 'Build completed successfully!'
            }
        }
    }
}
