pipeline {
    
    agent{
        label 'any'
    }
    

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
                sh 'mvn clean package'
            }
        }
    }
}
