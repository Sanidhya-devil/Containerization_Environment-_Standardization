pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                echo 'Repository cloned successfully.'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t containerization-project .'
            }
        }

        stage('Run Docker Container') {
            steps {
                bat '''
                docker rm -f containerization-project || exit 0
                docker run -d -p 8082:80 --name containerization-project containerization-project
                '''
            }
        }
    }
}
