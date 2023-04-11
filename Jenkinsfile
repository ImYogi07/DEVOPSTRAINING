pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "This is stage-1 on `hostname`"'
          }
        }

        stage('stage-1.1') {
          steps {
            sh '''sleep 5
echo "build is successfull for stage-1.1"'''
          }
        }

        stage('stage-1.2') {
          steps {
            sh '''sleep 5
echo "build is successfull for stage-1.2"'''
          }
        }

        stage('stage-1.3') {
          steps {
            sh '''sleep 5
echo "build is successfull for stage-1.1"'''
          }
        }

      }
    }

    stage('stage2') {
      parallel {
        stage('stage2') {
          steps {
            sh 'echo "this is stage-2 on `hostname`"'
          }
        }

        stage('stage-2.1') {
          steps {
            sh '''sleep 5
echo "build is successfull for stage-2.1"'''
          }
        }

      }
    }

  }
}