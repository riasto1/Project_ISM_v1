pipeline {
  agent any
  stages {
    stage('Build images') {
      steps {
        sh 'docker build -t myimage -f Dockerfile .'
      }
    }
  }
}