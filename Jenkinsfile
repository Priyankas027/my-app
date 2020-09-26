pipeline {
<<<<<<< HEAD
  agent any {
  label 'master'   
=======
  agent any 
>>>>>>> 46ccf0e8f713b2c0a7671ee2e045f89959600c42
    
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
       post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
    }
post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
}
