pipeline {
    agent any

    stages {
        stage('Build & Run App Inside Docker') {
            steps {
                script {
                    docker.image('node:18').inside {
                        sh 'node -v'
                        sh 'npm install'
                        sh 'npm run build || echo "no build script"'
                        sh 'docker build -t myapp .'
                        sh 'docker run -d -p 3000:3000 myapp'
                    }
                }
            }
        }
    }
}
