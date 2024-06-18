pipeline {
    agent any

    tools {
        nodejs "nodejs"
    }

    stages {
        stage('Install') {
            steps {
                sh 'yarn install'
            }
        }
        stage('Build') {
            steps {
                sh 'yarn build'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }

    post {
        success {
            echo "Success"
        }
        failure {
            echo "Error"
        }
    }
}