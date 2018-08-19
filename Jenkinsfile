pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Running Build Automation"
        sh './gradlew buil --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
