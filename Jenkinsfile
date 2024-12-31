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
                echo 'Compiling code...'
                sh 'g++ demo.cpp -o demo'  
            }
        }
        stage('Test') {
            steps {
                echo 'Running the program...'
                sh './demo' 
            }
        }
    }
}
