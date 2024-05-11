[11:31 PM] KHUSH VIRMANI .
pipeline {

    agent any

    stages {

        stage('Checkout') {

            steps {

                // Checkout code from Git repository

                git branch: 'main', credentialsId: 'kv_git', url: 'https://github.com/virmaniKhush/2023mt93176_devops.git'

            }

        }

        stage('Install Dependencies') {

            steps {

                // Install Node.js dependencies

                sh 'npm install'

            }

        }

        stage('Run Tests') {

            steps {

                // Run tests

                sh 'npm test'

            }

        }

        stage('Build') {

            steps {

                // Build the project 

                sh 'npm run build'

            }

        }

    }

}
