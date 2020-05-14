pipeline {
    agent any 
    stages {
        
      stage('Host comand execution') { 
           steps {
                sh "ls -a"
            }
      }  
      stage('Clone Repo and Clean') { 
           steps {
                sh "mvn clean"
            }
      }
       stage('Test') { 
           steps {
                 sh "mvn test"
            }
      }
       stage('Deploy') { 
           steps {
                 sh "mvn package"
            }
         }
    }
    
}
