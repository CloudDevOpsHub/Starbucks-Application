pipeline {
    agent any
    tools {
        jdk 'jdk17'
        nodejs 'node16'
    }
    stages {
        stage ("Clean Workspace") {
            steps {
                cleanWs()
            }
        }
        stage ("Git Checkout") {
            steps {
                git branch: 'main', url: 'https://github.com/CloudDevOpsHub/Starbucks-Application.git'
            }
        }
        stage("Install NPM Dependencies") {
            steps {
                sh "npm install"
            }
        }
        stage("Build Docker Image") {
            steps {
                sh "docker build -t starbucks ."
            }
        }
        stage("Tag & Push to DockerHub") {
            steps {
                script {
                    withDockerRegistry(credentialsId: 'docker') {
                        sh "docker tag starbucks rishi2911/starbucks:latest"
                        sh "docker push rishi2911/starbucks:latest"
                    }
                }
            }
        }
    }
}
