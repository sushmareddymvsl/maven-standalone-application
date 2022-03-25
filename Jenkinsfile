pipeline{  
  agent any
	def gitHome = tool name: "Git"
	def mavenHome = tool name: "maven 3.6.3"
  stages{
    stage('Welcome'){
      steps{
        echo 'Welcome'
      }
    }
    stage('CheckOutCode'){
    steps{
    git branch: 'master', credentialsId: 'GitHub', url: 'https://github.com/sushmareddymvsl/maven-standalone-application.git'
	
	}
  }
    stage('Build'){
  steps{
	  sh  "${mavenHome}/bin/mvn clean install"
  }
  }
 }
}
