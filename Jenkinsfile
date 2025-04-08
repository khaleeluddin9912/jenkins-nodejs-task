pipeline {
    agent {
        docker {
            image 'node:18'
            args '-p 3000:3000'
        }
    }

    stages {
        stage('Check Node and NPM') {
            steps {
                sh 'node -v'
                sh 'npm -v'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build App') {
            steps {
                sh 'npm run build || echo "No build script"'
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
