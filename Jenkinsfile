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
        sh 'docker run -p 3000:3000 myimage '
        input 'Finished using website?'
        sh 'docker stop myimage'
      }
    }
  }
}