pipeline {
    agent any

    stages {
        stage('Use Node Image') {
            steps {
                script {
                    docker.image('node:18').inside {
                        sh 'node -v'
                        sh 'npm -v'
                        sh 'npm install'
                        sh 'npm run build || echo "No build script"'
                        sh 'docker build -t myapp .'
                        sh 'docker run -d -p 3000:3000 myapp'
                    }
                }
            }
        }
    }
}
