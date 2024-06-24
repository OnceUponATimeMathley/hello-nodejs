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
                sh 'cat Dockerfile'
                // withDockerRegistry(credentialsId: 'dockerhub', url: 'https://index.docker.io/v1/') {
                    
                // }
            }
        }
    }
}
