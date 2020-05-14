pipeline {
    agent any 
    stages {
        
      stage('Host comand execution') { 
           steps {
                sh "for i in {2..4}; do echo $i;done && uptime"
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
