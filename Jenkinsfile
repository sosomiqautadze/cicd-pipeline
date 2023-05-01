pipeline {
  agent any
  stages {
    stage('Webhook') {
      steps {
        git(url: 'https://github.com/sosomiqautadze/cicd-pipeline.git', branch: 'main', poll: true)
      }
    }

    stage('test') {
      steps {
        sh 'npm install'
      }
    }

  }
}