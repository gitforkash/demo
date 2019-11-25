pipeline {
  agent any
  
  tools {
    maven 'Maven362'
  }
  stages {
    stage('Checkout'){
      steps {
        step("Step1") {
          git 'https://github.com/gitforkash/demo.git'
          sh 'echo "Checking out from SCM"'
        }
        
        step ("Step 2") {
          sh 'echo "This is another step named 2'
        }
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
