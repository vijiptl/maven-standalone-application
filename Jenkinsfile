pipeline {
    agent any
    
    environment {
        GIT_SSL_NO_VERIFY = 'true'  // Disable SSL verification globally
    }
    
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    echo 'Cloning the Git repository with SSL verification disabled...'
                    sh 'git config --global http.sslVerify false'
                    git url: 'https://github.com/vijiptl/maven-standalone-application.git', branch: 'master'
                }
            }
        }
    }
}
