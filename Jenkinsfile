pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                checkout scm
                echo 'getting... ' + env.GIT_BRANCH

            }
        }
    }
    post {
        failure {
            script {
                // CHANGE_ID is set only for pull requests, so it is safe to access the pullRequest global variable
                if (env.CHANGE_ID) {
                    pullRequest.addLabel('Build Failed')
                }
            }
        }
    }
}
