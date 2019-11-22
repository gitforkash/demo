pipeline {
  agent any
  
  stages {
    stage ('Checkout'){
      git 'https://github.com/gitforkash/demo.git'
      sh 'echo "Checking out from SCM"'
    }
    stage ('Build'){
      sh 'echo "Building this thing,, !"'
    }
  }
}
