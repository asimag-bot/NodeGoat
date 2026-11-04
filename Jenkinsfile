pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                echo '=== Step 1: GitHub-dan NodeGoat kodu kopyalanır ==='
            }
        }
        stage('SAST Dependency Scan') {
            steps {
                echo '=== Step 2: Layihədəki köhnə paketlər və təhlükəsizlik boşluqları skan olunur ==='
                echo '[CRITICAL] Found high-severity vulnerability in package: express (v3.0.0)'
                echo '[ERROR] Zəiflik tapıldığı üçün pipeline dayandırılır!'
                error('Təhlükəsizlik boşluğu tapıldı! Xahiş olunur kodu düzəldin.')
            }
        }
        stage('Deploy') {
            steps {
                echo '=== Step 3: Deploy olunur ==='
            }
        }
    }
}
