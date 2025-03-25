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
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                sh 'node index.js'
            }
        }
    }
}