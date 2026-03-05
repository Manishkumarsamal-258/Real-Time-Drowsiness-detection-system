pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Manishkumarsamal-258/Real-Time-Drowsiness-detection-system.git'
            }
        }

        stage('Check Python') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip3 install numpy scipy imutils opencv-python'
            }
        }

        stage('Verify Python Files') {
            steps {
                sh 'python3 -m compileall .'
            }
        }

    }
}
