pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the website...'
                // No build step needed for static HTML
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the website...'
                // Optional: Add tests for static HTML files, e.g., HTML validation
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the website to XAMPP...'
                // Copy files to the XAMPP htdocs directory
                sh 'cp -r * C:/xampp/htdocs/'
            }
        }
    }
    post {
        success {
            echo 'Deployment successful! Website is live.'
        }
        failure {
            echo 'Build or deployment failed.'
        }
    }
}
