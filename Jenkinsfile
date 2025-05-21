pipeline {
    agent any

    stages {
        stage('Preparation') {
            steps {
                echo 'Menyiapkan pipeline...'
            }
        }

        stage('Build') {
            steps {
                echo 'Tahap build dijalankan (simulasi)...'
                // Simulasi perintah build, bisa ganti sesuai kebutuhan
                sh 'echo "Build selesai."'
            }
        }

        stage('Test') {
            steps {
                echo 'Tahap test dijalankan (simulasi)...'
                // Simulasi perintah test
                sh 'echo "Test selesai."'
            }
        }
    }

    post {
        success {
            echo 'Build berhasil!'
        }
        failure {
            echo 'Build gagal!'
        }
    }
}
