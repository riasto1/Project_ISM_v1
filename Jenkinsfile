pipeline {
  agent {
    dockerfile true

  }
  stages {
    stage('Initialize'){
       def dockerHome = tool 'myDocker'
       env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
    
    stage('Run images') {
      steps {
        sh 'telnet'
      }
    }
  }
}
