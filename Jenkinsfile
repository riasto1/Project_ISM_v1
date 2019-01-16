pipeline {
  agent {
    dockerfile true
  }
  stages {
    stage('Initialize environment') {
      steps {
        script {
          def dockerHome = tool 'myDocker'

          env.PATH = "${dockerHome}/bin:${env.PATH}"
        }

      }
    }
    stage('Run images') {
      steps {
        sh 'myDocker run f29bab4cdb3a1259fa40c27f891efeb6424109b4 -p 3000:3000'
      }
    }
  }
}