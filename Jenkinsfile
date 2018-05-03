pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        echo 'current directory'
        sh 'pwd'
      }
    }
    stage('build infra') {
      steps {
        echo 'building infra'
        ws(dir: '/var/lib/jenkins/demo1') {
          sh '''cd /var/lib/jenkins/demo1
pwd
./iac_test_new.sh
'''
        }
        
      }
    }
  }
}