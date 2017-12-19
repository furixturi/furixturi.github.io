node {
    /* "Build" and "Test" stages omitted */

    stage('Deploy - Staging') {
        echo 'deploy staging'
    }

    stage('Sanity check') {
        input "Does the staging environment look ok?"
    }

    stage('Deploy - Production') {
       echo 'deploy production'
    }
}

