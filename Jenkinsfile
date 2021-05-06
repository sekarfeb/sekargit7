def code

pipeline {
agent any
 
   stages{
    
    
  stage('Load') {
   steps{
    script {
    code = load 'example.groovy'
  }
   }
    }

  stage('Execute') {
    code.example1()
  }
}


 }
