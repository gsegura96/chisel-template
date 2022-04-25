pipeline {
  agent any
  stages {
    stage('Initialize in Docker') {
      agent {
        docker {
          image 'mozilla/sbt'
        }
      }
      stages {
        stage('sbt test'){
          steps{
            echo "running sbt test"
            sh "sbt 'testOnly gcd.GcdDecoupledTester'"
          }
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
