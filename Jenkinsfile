pipeline{
   agent any
   tools {
        maven 'Apache Maven 3.6.0'
        jdk 'JDK 10'
   }
   stages {
      stage('Pull') { 
         steps{
           git 'https://github.com/samanbatoolInvesco/JenkinsTask.git'
         }
       }
      stage ('Build'){
         steps{
               bat "mvn clean compile"
         }
      }
	   stage ('Test'){
         steps{
               bat "mvn test"
         }
      }
   }
}
