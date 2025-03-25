pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/A-akarshanSharma/Calculator.git' // Replace with your repo URL
            }
        }
        stage('Build') {
            steps {
                sh 'g++ -o calc calc.cpp' // Compile C++ program
            }
        }
        stage('Test') {
            steps {
                sh './calc' // Run the compiled program
            }
        }
    }
}
