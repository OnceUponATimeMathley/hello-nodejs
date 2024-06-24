pipeline {
    agent any
    stages{
        stage('Clone') {
            steps {
                git 'https://github.com/OnceUponATimeMathley/hello-nodejs.git'
            }
        }

        stage('Build') {
            steps {
                withDockerRegistry(credentialsId: 'dockerhub_credential', url: 'https://index.docker.io/v1/') {
                    sh 'docker build -t onceuponatimemathley/jenkins:v1 .'
                }
            }
        }
    }
}
