pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'echo "This is stage-1 on `hostname`"'
      }
    }

    stage('stage2') {
      steps {
        sh 'echo "this is stage-2 on `hostname`"'
      }
    }

  }
}