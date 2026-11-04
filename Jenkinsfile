pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                echo '=== Step 1: GitHub reposundan kódlar çəkilir ==='
            }
        }
        stage('SAST & Vulnerability Scan') {
            steps {
                echo '=== Step 2: NodeGoat reposunda təhlükəsizlik skanı aparılır ==='
                echo '[INFO] Trivy / SAST skaneri işə düşdü...'
                echo '[WARN] Zəiflik tapıldı: Köhnə paketlər və zəif kod strukturu tespit edildi!'
            }
        }
        stage('Build & Deploy') {
            steps {
                echo '=== Step 3: Layihə uğurla derləndi ==='
            }
        }
    }
}
