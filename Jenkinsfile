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
   steps{
    script {
    code.example1()
    }
   }
  }
}
code.example2()

 }
