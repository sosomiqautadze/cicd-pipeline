pipeline {
  agent any
  stages {
    stage('Run') {
      steps {
        sh '''stage(RUN){
   sh ./scripts/build.sh 
}'''
        }
      }

    }
  }