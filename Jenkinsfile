pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repo...'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t nodejs-app .'
            }
        }

        stage('Docker Run') {
            steps {
                sh 'docker run -d -p 3000:3000 nodejs-app'
            }
        }
    }
}
