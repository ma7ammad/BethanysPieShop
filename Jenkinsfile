pipeline {
        agent any

    // agent {
    //     docker {
    //         image 'mcr.microsoft.com/dotnet/core/sdk:3.1.101'
    //     }
    // }

    stages {
        stage('Verify') {
            steps {
                sh '''
                  dotnet --list-sdks
                  dotnet --list-runtimes
                '''
                sh 'printenv'
                sh 'ls -l "$WORKSPACE"'
            }
        }
        stage('SCM') {
            steps {
                echo 'Gathering code from SCM'
                git branch: '${branch}', url: 'https://github.com/ma7ammad/BethanysPieShop'
            }
        }
        stage('Build') {
            steps {
                // sh 'dotnet --version'
                //sh 'dotnet build BethanysPieShop'
                echo 'Building Mo ...'
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