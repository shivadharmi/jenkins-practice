/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:latest' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
