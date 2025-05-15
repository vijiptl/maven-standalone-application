pipeline {
    agent any

    environment {
        // If you're dealing with SSL issues (e.g., self-signed certs), uncomment the next line:
        // GIT_SSL_NO_VERIFY = 'true'
    }

    stages {
        stage('List Repository Files') {
            steps {
                echo "Listing files in workspace..."
                sh 'ls -l'
            }
        }

        stage('Build') {
            steps {
                echo "Placeholder for your build commands"
                // For example:
                // sh './build.sh'
                // or for Maven:
                // sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo "Placeholder for your test commands"
                // For example:
                // sh 'npm test'
                // or for Java:
                // sh 'mvn test'
            }
        }

        stage('Archive Artifacts') {
            steps {
                echo "Archiving build outputs..."
                // Change path to match your build output
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the logs.'
        }
    }
}
