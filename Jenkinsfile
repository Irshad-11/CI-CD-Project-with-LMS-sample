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
                // Ensure we are in the Jenkins workspace directory
                sh 'pwd' // Optional: Print the current directory for debugging

                // Compile the C code
                bat "gcc -o LMS LMS_V1_0_1.c"
                // OR
                //sh "gcc -o LMS LMS_V1_0_1.c"

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
