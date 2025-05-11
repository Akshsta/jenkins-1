pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')  // Poll every 5 mins as fallback
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/your-org/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                // your build commands here (e.g., mvn clean install)
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                // your test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying to production..."
                // your deployment steps here
            }
        }
    }
}
