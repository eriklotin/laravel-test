pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "composer install"'

            }
        }
    }
    post {
        success {
            setBuildStatus("Build succeeded", "SUCCESS");
        }
        failure {
            setBuildStatus("Build failed", "FAILURE");
        }
      }
}
