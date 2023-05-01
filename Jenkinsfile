pipeline {
  agent {
    docker {
      args '3000:3000 '
      image 'node:lts-alpine'
    }

  }
  stages {
    stage('Run') {
      steps {
        sh 'sh \'./scripts/build.sh\''
      }
    }

    stage('Test') {
      steps {
        sh 'sh \'./scripts/test.sh\''
      }
    }

  }
}