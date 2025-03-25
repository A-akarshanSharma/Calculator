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
                sh 'g++ -o calculator calc.cpp' // Compile C++ program
            }
        }
        stage('Test') {
            steps {
                sh './calculator' // Run the compiled program
            }
        }
    }
}
