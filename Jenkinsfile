pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Hello, Jenkins! This is trial1'
            }
        }
    }
}
