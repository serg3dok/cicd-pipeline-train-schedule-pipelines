pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew --no-daemon'
        arhiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
