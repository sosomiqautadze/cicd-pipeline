pipeline {
  agent any
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

    stage('Build') {
      steps {
        dockerNode(image: 'nodejs:19')
      }
    }

  }
}