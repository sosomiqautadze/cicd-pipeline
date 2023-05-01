pipeline {
  agent none
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