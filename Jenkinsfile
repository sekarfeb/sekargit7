pipeline {
  agent any
  stages {
    stage ("Build"){
      steps{
        echo " Build Successfull"
      }
    }
    
    stage("Test"){
      when {
        expression{
          BRANCH_NAME=="main"
        }
      }
      steps{
        echo "Tsting successfull"
      }
    }
  
  
  
   stage("Deploy"){
      steps{
        echo "Deploy successfull"
      }
    }
  }
  
  post {
    always {
      echo "build completed"
    }
  }
}
