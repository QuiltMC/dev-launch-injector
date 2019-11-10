pipeline {
   agent any
   stages {

      stage('Init') {
         steps {
            sh "chmod +x gradlew"
         }
      }

      stage ('Build') {
         steps {
            sh "./gradlew clean build publish --refresh-dependencies --stacktrace"
         }
      }
   }
}