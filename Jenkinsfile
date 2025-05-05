pipeline {
    agent any

    environment {
        // Skip SSL verification for Git
        GIT_SSL_NO_VERIFY = 'true'
    }

    stages {
        stage('Clone Repository') {
            steps {
                script {
                    // Define the Git repository URL
                    def gitUrl = 'https://github.com/your-repository.git'

                    // Clone the Git repository without SSL verification
                    git url: gitUrl
                }
            }
        }

        // Additional stages can be added here if needed
    }
}
