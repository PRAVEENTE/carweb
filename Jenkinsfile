pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
               git branch: 'main', url: 'https://github.com/PRAVEENTE/carweb.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
            }
        }

        stage('Deploy') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}
