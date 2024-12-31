pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/your-username/your-repo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling code...'
                sh 'g++ test.cpp -o test'
            }
        }
        stage('Test') {
            steps {
                echo 'Running the program...'
                sh './test'
            }
        }
    }
}
