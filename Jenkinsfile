pipeline {
  agent any
  stages {
    stage('env') {
      steps {
        sh 'echo $JOB_NAME |cut -d / -f 2 >/tmp/111'
      }
    }
    stage('checkjname') {
      steps {
        sh 'cat /tmp/111'
      }
    }
  }
}