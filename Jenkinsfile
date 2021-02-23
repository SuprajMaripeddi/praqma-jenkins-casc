node {
    
    checkout([
         $class: 'GitSCM',
         branches: scm.branches,
         doGenerateSubmoduleConfigurations: scm.doGenerateSubmoduleConfigurations,
         extensions: scm.extensions,
         userRemoteConfigs: scm.userRemoteConfigs
    ])
    stage('scm'){
        echo 'Pulling... ' + env.GIT_BRANCH

    }
    
 
    }
