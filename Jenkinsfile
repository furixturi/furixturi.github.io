node {
    stage('Build') {
        echo 'Building'
    }
    stage('Test') {
        echo 'Testing'
    }
    stage('Deploy - Staging') {
        sh './deploy staging'
        sh './run-smoke-tests'
    }
    stage('Sanity check') {
        input "Does the staging environment look ok?"
    }
    stage('Deploy - Production') {
        sh './deploy production'
    }
}