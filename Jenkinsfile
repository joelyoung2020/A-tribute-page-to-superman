pipeline {
  agent any
  stages {
    stage("run frontend") {
      steps {
        echo 'excuting yarn'
        nodejs('Node-10') {
          sh 'yarn install'
        }
      }
   }
    stage("run frontend") {
      steps {
        echo 'excuting graddle'
        withGradle() {
          sh './gradlew -v'
        }
      }
   }
}

