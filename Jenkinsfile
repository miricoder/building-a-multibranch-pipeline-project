pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'sudo npm install --unsafe-perm=true --allow-root'
            }
        }
        stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}