pipeline {
    agent any   // runs on any available Jenkins agent

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/<your-username>/jenkins-pipeline-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "🔨 Building the project..."
            }
        }

        stage('Test') {
            steps {
                echo "🧪 Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Deploying application..."
            }
        }
    }

    post {
        success {
            echo "✅ Pipeline finished successfully!"
        }
        failure {
            echo "❌ Pipeline failed!"
        }
    }
}
