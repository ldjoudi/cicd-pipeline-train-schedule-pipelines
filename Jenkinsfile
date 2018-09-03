pipeline {
  agent any
  stages {
    stage ('build') {
      step {
        eho 'Running Build Automation'
        sh './gradlew build --no daemon'
        archiveArtifacts artifacts: '/dist/trainSchedule.zip'
      }
    }
  }
}
