pipeline {
    agent any

    stages {
        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("deividlm/kube-news:${env.BUILD_id}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}