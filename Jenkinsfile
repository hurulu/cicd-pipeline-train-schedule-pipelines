pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Running automatic build"
        sh "./gradlw build --no-daemon"
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
