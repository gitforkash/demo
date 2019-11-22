pipeline {
  agent any
  
  tools {
    maven 'Maven362'
  }
  stages {
    stage('Checkout'){
      steps {
        git 'https://github.com/gitforkash/demo.git'
        sh 'echo "Checking out from SCM"'
      }
    }
    stage ('Compile'){
      steps{
        sh 'echo "Compiling this thing,, !"'
        sh 'mvn compile'
      }
    }
    stage ('Test'){
      steps{
        sh 'echo "Testing this thing,, !"'
        sh 'mvn test'
      }
    }
    stage ('Package'){
      steps{
        sh 'echo "packaging this thing,, !"'
        sh 'mvn package'
      }
    }
  }
}
