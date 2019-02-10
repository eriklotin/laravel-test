pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'whoami'
                sh 'id'
                sh 'echo 5'
                sh 'docker run --rm -v "`pwd`:/var/www" eriklotin/workspace composer install'
            }
        }
    }
}
