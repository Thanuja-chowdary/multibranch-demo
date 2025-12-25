pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Build stage running on branch: ${env.master}"
            }
        }

        stage('Test') {
            steps {
                echo "Test stage running on branch: ${env.master}"
            }
        }

        stage('Deploy') {
            when {
                branch 'master'
            }
            steps {
                echo "Deploying to PRODUCTION (master  branch only)"
            }
        }
    }
}

