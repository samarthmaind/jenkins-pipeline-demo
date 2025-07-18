pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                echo "Cloning code from GitHub..."
                git branch: 'main', url: 'https://github.com/samarthmaind/jenkins-pipeline-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Running build stage..."
                sh 'python3 app.py'
            }
        }

        stage('Test') {
            steps {
                echo "Running test stage..."
                sh 'chmod +x test.sh && ./test.sh'
            }
        }
    }
}
