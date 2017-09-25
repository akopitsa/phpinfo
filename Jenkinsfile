node('HetznerStage') {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */
        checkout scm
    }
   echo 'Hello World'
   stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */
pipeline {
    agent {
        docker { image 'php:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'php --version'
            }
        }
    }
}
        /*app = docker.build("php") */
    }
}
