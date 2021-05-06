pipeline {
  agent any
  
  tools{
    maven 'myMaven'
  }
  
  environment{
    New_Version = '1.0.0'
  }
  stages {
    stage ("Build"){
      steps{
        echo " Build Successfull"
        echo  "Building Version number ${env.New_Version}"
        sh 'mvn install'
       
      }
    }
    
    stage("Test"){
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
