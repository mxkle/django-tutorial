pipeline {
  agent {
    docker {
      image 'python:3'
      args '-v /app:/app -p 5000:5000'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'python3 app/myproject/manage.py runserver 0:5000'
      }
    }
  }
}