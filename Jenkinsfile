pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t containerization-project .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh '''
                docker rm -f containerization-project || true
                docker run -d -p 8082:80 --name containerization-project containerization-project
                '''
            }
        }
    }
}
