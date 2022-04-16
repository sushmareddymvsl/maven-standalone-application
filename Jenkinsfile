pipeline{  
  agent any
	tools{
maven 'Maven'

}

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
	  sh  "mvn clean package"
  }
  }
 }
}
