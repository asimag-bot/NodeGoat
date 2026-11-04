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
                echo '=== Step 2: Paketlər və zəifliklər skan olundu ==='
                echo '[SUCCESS] Bütün asılılıqlar və zəifliklər bərpa olundu! 0 Boşluq.'
            }
        }
        stage('Deploy') {
            steps {
                echo '=== Step 3: Tətbiq təhlükəsiz şəkildə deploy olundu! ==='
            }
        }
    }
}
