pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "composer install"'
                bitbucketStatusNotify ( buildState: 'SUCCESSFUL' )
            }
        }
    }
}
