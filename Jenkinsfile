pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '\'${mvnHome}/bin/mvn clean install -f helloworld/pom.xml\''
      }
    }
  }
  environment {
    tool = 'maven'
  }
}