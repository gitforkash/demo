pipeline {
  agent any
  
  tools{
    maven 'M3'
  }
  stages {
    stage ('Checkout'){
      steps{
        git 'https://github.com/gitforkash/demo.git'
        sh 'echo "Checking out from SCM"'
      }
    }
    stage ('Build'){
      steps{
        sh 'echo "Building this thing,, !"'
      }
    }
  }
}
