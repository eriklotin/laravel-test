pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'whoami'
                sh 'id'
                sh 'echo 1'
                sh "echo ${workspace}"
                sh 'echo ${env.JOB_NAME}'
                sh 'echo ${env}'
                sh 'docker run --rm -v "`pwd`:/var/www" eriklotin/workspace composer install'
            }
        }
    }
}
