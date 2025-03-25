pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/mechbrian024/jenkinssample.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run App') {
            steps {
                bat 'node index.js'
            }
        }
    }
}