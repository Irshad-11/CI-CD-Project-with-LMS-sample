pipeline {
    agent any  // Runs the pipeline on any available agent

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Irshad-11/CI-CD-Project-with-LMS-sample'
            }
        }

        stage('Build') {
            steps {
                script {
                    bat '''
                    cd "F:\\Document\\Irshad_01\\BDU things\\Official\\Software Engineering\\LMS Project"
                    gcc -o LMS LMS.c
                    '''
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    bat '''
                    cd "F:\\Document\\Irshad_01\\BDU things\\Official\\Software Engineering\\LMS Project"
                    LMS.exe
                    '''
                }
            }
        }
    }
}
