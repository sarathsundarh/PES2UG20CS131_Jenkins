pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      
      sh 'g++ -o test test.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './test'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}


