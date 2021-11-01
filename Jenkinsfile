pipeline {
  agent any
  stages {
    stage ("Build") {
      steps { 
        echo "The automated build is in progress."
        sh "./gradlew build --no-daemon"
        archiveArtifacts artifacts: "dist/trainSchedule.zip"
      }
    } 
  }
}
