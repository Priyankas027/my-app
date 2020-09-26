pipeline {

  agent any
  
    options {
        timeout(time: 20, unit: 'SECONDS')
    }
    stages {
        stage('---clean---') {
            steps {
                sh "mvn clean"
            }
        }
        
        stage('--package--') {
            steps {
                sh "mvn package"
            
            }
        }
       stage('--Demo--') {
            steps {
                sh "ps -ef"
      
            }}
     
    }
 post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
}
