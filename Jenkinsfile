pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'whoami'
                sh 'id'
                sh 'echo 4'
                sh 'docker run --rm -v "`pwd`:/var/www" eriklotin/workspace composer install'
            }
        }
    }
}
