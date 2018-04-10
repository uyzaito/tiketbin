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
        jiraComment(issueKey: 'TPJ-1', body: 'se realizo el build "${BUILD_NUMBER}"')
      }
    }
  }
  tools {
    maven 'maven'
    jdk 'java'
  }
}
