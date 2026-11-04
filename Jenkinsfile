pipeline {
    agent any

    stages {
        stage('Code Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/asimag-bot/NodeGoat.git'
            }
        }
        
        stage('OWASP / SAST Dependency Scan') {
            steps {
                echo '=== OWASP Audit / SAST Skanı Başladılır ==='
                // Real zəiflikləri skan edir və kritik boşluq tapılarsa pipeline-ı avtomatik dayandırır
                sh 'npm audit --audit-level=high'
            }
        }

        stage('Deploy') {
            steps {
                echo '=== Step 3: Tətbiq uğurla deploy olundu ==='
            }
        }
    }
}
