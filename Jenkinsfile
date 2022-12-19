pipeline{
    agent any
    
    triggers {
  pollSCM '* * * * *'
   }
    
    stages{
        stage("git code"){
            steps{
                git 'https://github.com/manikantanukala-devops/SnapShot.git'
            }
        }
        stage("creating build"){
            steps{
                sh "npm install"
            }
        }
        stage("starting application"){
            steps{
                sh "npm start &"
            }
        }
        
        
    }
}
