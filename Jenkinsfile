pipeline {
    
    agent{
        label 'FirstNode'
    }
    

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "maven-3.x"
    }
    
   
    

    stages {
        stage('pull the code form scm') {
            steps {
                // Get some code from a GitHub repository
                git branch: "${BRANCH}",
                credentialsId: 'github-creds',
                url: 'https://github.com/Saleem313/devops-maven-web-app.git'

              
            }
        }
        
        stage('build'){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}
