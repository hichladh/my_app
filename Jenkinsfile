pipeline {
  agent any

  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/hichladh/my-app.git'
      }
    }

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
