pipeline {
    agent any

    stages {
        stage('SCM') {
            steps {
                echo 'Gathering code from SCM'
                git branch: '${branch}', url: 'https://github.com/ma7ammad/BethanysPieShop'
            }
        }
        stage('Build') {
            steps {
                sh 'dotnet --version'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Mo ...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Mo ...'
            }
        }
    }
}