pipeline {
    agent any
    stages {
        stage ('push docker stage') {
            steps {
                withDockerRegistry(credentialsId: 'dockerhub', url: 'https://index.docker.io/v1/') {
                    echo 'Hello world'
                }
            }
        }
    }
}
