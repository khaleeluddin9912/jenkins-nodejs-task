pipeline {
    agent any

    stages {
        stage('Print Node & NPM Versions') {
            steps {
                sh 'node -v || echo "Node not installed"'
                sh 'npm -v || echo "NPM not installed"'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install || echo "npm install failed"'
            }
        }

        stage('Build App') {
            steps {
                sh 'npm run build || echo "no build script found"'
            }
        }

        stage('Docker Build & Run') {
            steps {
                sh 'docker build -t myapp .'
                sh 'docker run -d -p 3000:3000 myapp'
            }
        }
    }
}
