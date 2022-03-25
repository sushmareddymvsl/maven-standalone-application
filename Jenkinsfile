pipeline{  
  agent any
  stages{
    stage'(Welcome'){
      steps{
        echo 'Welcome'
      }
    }
    stage('CheckOutCode'){
    steps{
    git branch: 'master', credentialsId: '957b543e-6f77-4cef-9aec-82e9b0230975', url: 'https://github.com/devopstrainingblr/maven-web-application-1.git'
	
	}
  }
    stage(Build){
      steps{
        sh mvn clean install
