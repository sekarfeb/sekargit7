pipeline {
  agent any
  stages {
    stage ("Build"){
      steps{
        echo " Build Successfull"
        echo  env.BRANCH_NAME
      }
    }
    
    stage("Test"){
      when {
        expression{
          env.BRANCH_NAME=='main'
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
