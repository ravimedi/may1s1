pipeline {
  agent any
  stages {
    stage('env') {
      steps {
        sh '''JNAME=$(echo $JOB_NAME |cut -d / -f 2)
export JNAME'''
      }
    }
    stage('checkjname') {
      steps {
        sh 'echo $JNAME'
      }
    }
  }
}