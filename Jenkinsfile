pipeline {
    
    /*agent{
        label 'any'
    }*/

    agent any
    

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "m399"
    }
    
   
    

    stages {
        /*stage('pull the code form scm') {
            steps {
                // Get some code from a GitHub repository
                git branch: 'master',
                credentialsId: 'github-creds',
                url: 'https://github.com/Saleem313/devops-maven-web-app.git'

              
            }
        }*/
        
        stage('build'){
            steps{
              script{ 
               for(i=1; i<70; i++){
                   echo "${i+1}"
                   sleep 1
               }
                sh 'mvn clean package'
            }
           }
        }
    }
}
