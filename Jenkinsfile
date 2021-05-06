pipeline {
  agent any
  
  parameters{
    string(name:'version',defaultValue:'2.0.0',description:'ssss')
  }
  
  environment{
    New_Version = '1.0.0'
  }
  stages {
    stage ("Build"){
      steps{
        echo " Build Successfull"
        echo  "Building Version number ${env.New_Version}"
        echo "${version}"
       
       
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
