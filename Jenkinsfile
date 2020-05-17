node {
   stage ('SCM Checkout'){
     git 'https://github.com/mani793/hello-world'
   }
   stage ('Compile-package'){
     def mvnHome = tool name: 'maven-3', type: 'maven' 
      sh "${mvnHome}/bin/mvn package"
   }  
   stage ('slack notify'){
   slackSend baseUrl: 'https://hooks.slack.com/services/', channel: '#jenkins-pipe-test', color: 'good', message: 'welcome to jenkins slack', teamDomain: 'WFH-testing', tokenCredentialId: 'slack-demo'
   }
}   
