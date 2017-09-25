node('HetznerStage') {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */
        checkout scm
    }
    docker.image('php:latest').inside {

    stage("Install Bundler") {
      sh "php -v"
    }

    stage("Use Bundler to install dependencies") {
      sh "hostname"
    }
    }
}
