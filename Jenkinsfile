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
        dockerNode(image: '16.13.1-alpine') {
          sh 'sh \'docker build -t myimage .\''
        }

      }
    }

  }
}