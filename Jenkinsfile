pipeline {
  agent any

  stages {
    stage("Build") {
      steps {
        echo 'build'
         withMaven(maven: 'mvn') {
            sh "mvn clean package"
        }
      }
    }

    stage("Test") {
      steps {
        echo 'test'
      }
    }
  }
}
