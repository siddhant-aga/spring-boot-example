pipeline {
    agent any
    stages {
        stage('Back-end') {
            steps {
                withDockerContainer('maven:3-alpine') {
                sh 'mvn --version'
                }
            }
        }
        stage('Front-end') {
            steps {
                withDockerContainer('node:7-alpine') {
                sh 'node --version'
                }
            }
        }
    }
}
