node('jenkins-slave') {
    stage('Back-end') {
            steps {
                withDockerContainer('maven:3-alpine') {
                sh 'mvn --version'
                }
            }
        }
    stage('Build'){
        container('go-agent') {
            // This is where we build our code.
        }
    }
}
