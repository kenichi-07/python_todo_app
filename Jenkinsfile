pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'dev', url: 'https://github.com/kenichi-07/python_todo_app.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'python3 -m unittest discover -s tests'
            }
        }
        stage('Deploy') {
            when {
                branch 'dev'
            }
            steps {
                echo 'Deploying to Development Environment...'
                // Add other deployment commands here
            }
        }
    }
    post {
        success {
            echo 'Build succeeded!'
            // Optional: Add notification steps
        }
        failure {
            echo 'Build failed!'
            // Optional: Add notification steps
        }
    }
}
