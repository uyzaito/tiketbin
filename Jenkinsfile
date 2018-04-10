pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '\'/var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/maven/mvn clean install -f helloworld/pom.xml\''
      }
    }
  }
  tools { 
        maven 'maven' 
        jdk 'java'
  }
}
