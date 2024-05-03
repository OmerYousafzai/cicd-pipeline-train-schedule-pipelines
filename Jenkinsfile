pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
   stage ('Test') {
     steps {
       echo 'This is just a test'
       sh 'date'
     }
   }
  }
}
