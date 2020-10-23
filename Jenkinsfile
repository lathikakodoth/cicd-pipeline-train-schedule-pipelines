pipeline {
    agent any
    stages{
       stage ('Build'){
           steps{
               Running "gradle build ...."
               sh './gradlew build --no-daemon'
               archiveArtifacts 'dist/trainSchedule.zip'

           }
       }
   }
}
