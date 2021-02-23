node {
    stage('checkout'){
        checkout scm
    }
    stage('shell') {
            steps {
                sh 'echo env.BRANCH_NAME' 
            }
    }
}
