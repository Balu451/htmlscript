pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the website...'
                // Optionally, perform additional build tasks here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the website...'
                // Optionally, add automated tests here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the website...'
                bat '''
                    del /Q "C:\\xampp\\htdocs\\*"
                    xcopy /E /I * "C:\\xampp\\htdocs\\"
                '''
            }
        }
    }
}
