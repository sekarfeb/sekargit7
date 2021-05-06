pipeline {
  agent any
  stages {
    stage ("Build"){
      steps{
        echo " Build Successfull"
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
