pipeline {
  agent any
  stages {
    stage('Build images') {
      steps {
        sh 'docker build -t myimage -f Dockerfile .'
      }
    }
    stage('Run images') {
      steps {
        sh 'docker run myimage -p 3000:3000'
      }
    }
  }
}