pipeline {
  agent any
  stages {
    stage('1123') {
      steps {
        sh '''ls
echo
sleep 1'''
        echo 'sss'
        build(job: 'jobname', propagate: true, quietPeriod: 123, wait: true)
      }
    }

    stage('stage2') {
      steps {
        build(job: 'job2', propagate: true, quietPeriod: 1, wait: true)
      }
    }

  }
}