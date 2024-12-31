pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/22127159-22127229/Project3.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building project...'
                sh 'echo Build simulation' // thay thế lệnh build cụ thể nếu cần
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo Test simulation' // thay thế lệnh test nếu cần
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo Deploy simulation'
            }
        }
    }
}