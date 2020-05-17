node {
   stage ('SCM Checkout'){
     git 'https://github.com/mani793/hello-world'
   }
   stage ('Compile-package'){
     def mvnHome = tool name: 'maven-3', type: 'maven' 
      sh "${mvnHome}/bin/mvn package"
   }  
}   
