pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Perform build steps here
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                // Perform test steps here
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                // Perform deployment steps here
                sh 'npm run deploy'
            }
        }
    }

    post {
        success {
            // Actions to perform when the pipeline is successful
            echo 'Pipeline executed successfully'
        }

        failure {
            // Actions to perform when the pipeline fails
            echo 'Pipeline failed'
        }

        always {
            // Actions to always perform, regardless of the pipeline result
            echo 'Pipeline finished'
        }
    }
}
