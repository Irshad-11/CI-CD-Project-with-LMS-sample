pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Irshad-11/CI-CD-Project-with-LMS-sample'
            }
        }
        stage('Build') {
            steps {
                // Compile the C code using the 'bat' step for Windows
                bat "gcc -o LMS LMS_V1_0_1.c"

            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
            }
        }
    }
}
