pipeline {
  agent any

  stages {
    stage("Build") {
      steps {
        echo 'build'
         withMaven(maven: 'Maven3.8') {
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
