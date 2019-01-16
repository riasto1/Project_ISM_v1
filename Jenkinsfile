pipeline {
  agent {
    dockerfile true
    
    enviroment {
      def dockerHome = tool 'myDocker'
      env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
    
  }
  stages {
    
    stage('Run images') {
      
      steps {
        sh 'docker run f29bab4cdb3a1259fa40c27f891efeb6424109b4 -p 3000:3000'
      }
    }
  }
}
