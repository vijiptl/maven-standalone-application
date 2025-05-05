pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                script {
                    echo 'Cloning the Git repository with SSL verification disabled...'
                    git url: 'https://github.com/vijiptl/maven-standalone-application.git', branch: 'main'
                }
            }
        }
    }
}
