pipeline {
  agent any
  
  parameters{
    string(name:'version',defaultValue:'2.0.0',description:'ssss')
    booleanParam(name:'execute',defaultValue:'true',description:'Execute')
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
      when {
        expression{
          params.execute
        }
      }
         steps{
        echo "Tsting successfull"
      }
    }
  
  
  
   stage("Deploy"){
     
     script {
       def varia = load "script.groovy"
       varia.add()
     }
     
    }
  }
  
  post {
    always {
      echo "build completed"
    }
  }
}
