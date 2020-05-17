node {
   stage ('SCM Checkout'){
     git 'https://github.com/mani793/hello-world'
   }
   stage ('Compile-package'){
     sh 'mvn package'
   }  
}   
