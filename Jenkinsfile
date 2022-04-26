pipeline {
  agent any
  stages {
    
    stage('build') {
      steps {
        echo 'Building the application'
      }
    }
    
    stage('test') {
      steps {
        echo 'Testing the application'
        sh "sbt 'testOnly gcd.GcdDecoupledTester'"
      }
    }
    
    stage('deploy') {
      steps {
        echo 'Deploying the application'
      }
    }
  }
}
