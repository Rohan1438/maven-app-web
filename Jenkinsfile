pipeline{
  agent any
  
  environment{
    PATH = "$PATH:/opt/apache-maven-3.6.3/bin"
  }
stages{
   stage('GetCode'){
     steps{
       git branch : 'master'
       url : 'https://github.com/Rohan1438/maven-app-web.git'
     }
   } 
  stage('Build'){
    steps{
      sh 'mvn clean package'
    }
  }
}
}
