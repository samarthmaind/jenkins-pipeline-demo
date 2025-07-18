pipeline {
  agent any

  stages {

    stage('Clone Repository') {
      steps {
        echo "Cloning code from GitHub..."
        git 'https://github.com/samarthmaind/jenkins-pipeline-demo.git'
      }
    }

    stage('Build') {
      steps {
        echo "Building the application..."
        sh 'echo Simulating build step'
      }
    }

    stage('Test') {
      steps {
        echo "Running tests..."
        sh './test.sh'
      }
    }
  }
}
