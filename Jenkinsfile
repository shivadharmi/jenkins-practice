/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'node:latest' } }
    stages {
        stage('Initialize'){
            def dockerHome = tool 'myDocker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
        }
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
