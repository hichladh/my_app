pipeline {
  agent {
    docker {
      image 'python:3.10'   // official Python image with pip and pytest pre-installed or install pytest in your requirements.txt
    }
  }

  stages {
    stage('Install dependencies') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }

    stage('Run tests') {
      steps {
        sh 'pytest tests/'
      }
    }
  }
}
