pipeline {
    agent any

    stages {
        stege ('Build Docker Image') {
            seteps{
                script {
                    dockerapp = docker.build("deividlm/kube-news:${env.BUILD_id}", '-f ./src/DockerFile ./src')
                }
            }
        }
    }
}