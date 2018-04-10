pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn clean install -f "${WORKSPACE}"/helloworld/pom.xml'
      }
    }
    stage('jira') {
      steps {
        jiraSearch 'TPJ-1'
      }
    }
  }
  tools {
    maven 'maven'
    jdk 'java'
  }
}