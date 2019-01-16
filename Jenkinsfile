pipeline {
  agent {
    dockerfile true
  }
  stages {
    stage('Run images') {
      steps {
        script {
          def dockerHome = tool 'myDocker'

          env.PATH = "${dockerHome}/bin:${env.PATH}" docker ps
        }

        sh 'docker run f29bab4cdb3a1259fa40c27f891efeb6424109b4 -p 3000:3000'
      }
    }
  }
}