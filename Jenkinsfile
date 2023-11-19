pipeline {
    agent any
    stages {
        stage ('clone') {
            steps {
                git branch: 'main', url: 'https://github.com/duyhienn2012/testdocker.git'
            }
        }
        stage ('push docker stage') {
            steps {
                withDockerRegistry(credentialsId: 'dockerhub', url: 'https://index.docker.io/v1/') {
                    echo 'Hello world'
                }
            }
        }
    }
}
