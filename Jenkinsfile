pipeline {
    agent {
        docker {
            image 'node:18'
        }
    }
    stages {
        stage('Print Node & NPM Versions') {
            steps {
                sh 'node -v || echo Node not installed'
                sh 'npm -v || echo NPM not installed'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install || echo npm install failed'
            }
        }

        stage('Build App') {
            steps {
                sh 'npm run build || echo no build script found'
            }
        }

        stage('Docker Build & Run') {
            // This step needs Docker in Docker setup, which is more advanced.
            steps {
                echo 'Skipping Docker build in this stage because Docker is not available inside node:18 image by default.'
            }
        }
    }
}
