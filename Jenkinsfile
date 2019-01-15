pipeline {
  agent {
    dockerfile true
  }
  stages {
    stage('Run images') {
      steps {
        sh 'docker ps'
      }
    }
  }
}