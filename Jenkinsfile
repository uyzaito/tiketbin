pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn clean install -f "${WORKSPACE}"/helloworld/pom.xml'
      }
    }
  }
  tools { 
        maven 'maven' 
        jdk 'java'
  }
}
