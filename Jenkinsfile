pipeline {
  agent {
    dockerfile {
      filename 'dockerfile'
    }

  }
  stages {
    stage('Test') {
      steps {
        sh 'echo "Hello"'
      }
    }
  }
}