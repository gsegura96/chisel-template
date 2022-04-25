pipeline {
  agent any
  stages {
    stage('Initialize in Docker') {
      agent {
        docker {
          image 'mozilla/sbt'
        }
      }
    }
    
    stage('build') {
      steps {
        echo 'Building the application'
      }
    }
    
    stage('test') {
      steps {
        echo 'Testing the application'
      }
    }
    
    stage('deploy') {
      steps {
        echo 'Deploying the application'
      }
    }
  }
}
