pipeline {
  agent any
  triggers { pollSCM('*/1 * * * *') } // poll every minute for demo
  options { timestamps() }
  stages {
    stage('Build') {
      steps {
        echo 'Build: compiling & packaging (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
    stage('Unit & Integration Tests') {
      steps {
        echo 'Unit tests (demo)'
        sleep time: 1, unit: 'SECONDS'
        echo 'Integration tests (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
    stage('Code Analysis') {
      steps {
        echo 'Static code analysis (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
    stage('Security Scan') {
      steps {
        echo 'Security scan (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
    stage('Deploy to Staging') {
      steps {
        echo 'Deploy to staging (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
    stage('Integration Tests on Staging') {
      steps {
        echo 'Staging integration tests (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
    stage('Deploy to Production') {
      steps {
        echo 'Deploy to production (demo)'
        sleep time: 1, unit: 'SECONDS'
      }
    }
  }
  post {
    success { echo 'Finished: SUCCESS' }
  }
}
