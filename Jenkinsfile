pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Ganucj98/hello-world.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t hello-world .'
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run --rm hello-world'
            }
        }
    }
}
