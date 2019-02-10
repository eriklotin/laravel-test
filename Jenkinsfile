pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker run --rm -v "`pwd`:/var/www" eriklotin/workspace composer install'
            }
        }
    }
}
