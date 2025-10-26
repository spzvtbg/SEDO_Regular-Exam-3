pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                branch 'main'
            }
            steps {
                bat 'dotnet build'
            }
        }
        stage('Test') {
            when {
                branch 'main'
            }
            steps {
                bat 'dotnet test --no-build'
            }
        }
    }
}