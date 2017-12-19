pipeline {
    agent any
    stages {
        stage('Deploy') {
            timeout(time: 1, unit: 'MINUTES') {
                retry(5) {
                    sh './flakey-deploy.sh'
                }
            }
        }
    }
}