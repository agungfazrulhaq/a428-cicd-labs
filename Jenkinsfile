node{
    checkout scm
    docker.image('node:16-buster-slim').withRun('-p 3000:3000 --network=host'){
        stage('Build') {
            sh 'ls'
        }
        stage('Test') {
            sh './jenkins/scripts/test.sh'
        }
    }
}