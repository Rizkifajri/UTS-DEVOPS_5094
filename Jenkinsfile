pipeline {
    agent any

    tools {
        nodejs "NodeJS 18"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'development', url: 'https://github.com/Rizkifajri/UTS-DEVOPS_5094.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Unit Test') {
            steps {
                sh 'npm test'
            }
        }
    }

    post {
        success {
            echo 'Build sukses!'
        }
        failure {
            echo 'Build gagal!'
        }
    }
}
