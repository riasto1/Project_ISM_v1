pipeline {
  agent none
  stages {
    stage('Run images') {
      agent {
        dockerfile true
      }
      steps {
        sh 'docker run f29bab4cdb3a1259fa40c27f891efeb6424109b4 -p 3000:3000'
      }
    }
    stage('Initialize') {
      agent any
      steps {
        script {
          def dockerHome = tool 'myDocker'

          env.PATH = "${dockerHome}/bin:${env.PATH}"
        }

      }
    }
  }
}