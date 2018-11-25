pipeline{
   agent any
   tools {
        maven 'Apache Maven 3.6.0'
        jdk 'JDK 10'
   }
   stages {
      stage('Pull') { 
         steps{
           git 'https://github.com/talhakhannnnn/jenkins-practice-repo.git'
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
