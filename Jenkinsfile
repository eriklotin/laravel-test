pipeline {
    agent {
        docker { image 'eriklotin/workspace' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'composer install'
            }
        }
    }
}
