pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                // Jenkins clones automatically when configured from SCM
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test' // make sure your package.json has a test script
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying app...'
                sh 'echo Deploy step here!' // you can later replace this with real deployment logic
            }
        }
    }
}
