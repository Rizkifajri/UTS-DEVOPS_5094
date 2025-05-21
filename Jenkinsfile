pipeline {
    agent any

    tools {
        nodejs 'NodeJS 18' // harus sama dengan nama yang kamu isikan
    }

    stages {
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }

    post {
        failure {
            echo 'Build gagal!'
        }
    }
}
