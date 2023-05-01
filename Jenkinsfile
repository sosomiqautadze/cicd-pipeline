pipeline {
  agent any
  stages {
    stage('Run') {
      steps {
        sh '''stage(name){
   sh ./scripts/build.sh 
}'''
        }
      }

    }
  }