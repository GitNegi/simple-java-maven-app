pipeline {
    agent none
    stages{
        stage('dev_env'){
            agent { label 'mymaven' }
            steps{
                //sh 'date'
                git 'https://github.com/GitNegi/simple-java-maven-app.git'
                sh 'mvn package'
                sh 'java -jar target/*.jar'
                sh 'echo i am developer nodes'
            } // end of steps
        } // end of stage1
        
      
        
        
        
    } // end of stages
} // end of pipeline
