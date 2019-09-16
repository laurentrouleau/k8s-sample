pipeline {
agent any
stages {
         stage("Prepare"){ (3)
       steps{
         sh '''
           echo "debut de mon script"
           '''
         }
     }

     stage ("Build"){
       steps {
         sh '''
           echo "Building app"
         '''
       }
     }
}