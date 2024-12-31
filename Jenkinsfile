pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/22127159_22127229/Project3.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling code...'
                bat 'g++ demo.cpp -o demo.exe'
            }
        }
        stage('Test') {
            steps {
                echo 'Running the program...'
                bat './demo.exe'
            }
        }
    }
}
