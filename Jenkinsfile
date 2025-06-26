pipeline {
  agent any



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
