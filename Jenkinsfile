pipeline {
    agent none
    stages{
        stage('git'){
            agent { label 'mymaven' }
            steps{
                //sh 'date'
                git 'https://github.com/GitNegi/simple-java-maven-app.git'
                sh 'mvn package'
                sh 'java -jar target/*.jar'
                sh 'echo production  environment'
                
            }
        }
        
    
        
        
    }
}
