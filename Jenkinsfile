pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        powershell 'C:\\\\Users\\\\sony\\\\Desktop\\\\gradle-5.6-bin\\\\gradle-5.6\\\\bin\\\\gradle build'
        powershell 'C:\\\\Users\\\\sony\\\\Desktop\\\\gradle-5.6-bin\\\\gradle-5.6\\\\bin\\\\gradle javadoc'
        archiveArtifacts 'build/libs/*.jar'
        archiveArtifacts 'build/docs/javadoc/*'
      }
    }

  }
}