pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '/var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/maven/bin/mvn clean install -f "${WORKSPACE}/helloworld/pom.xml'
      }
    }
  }
  tools { 
        maven 'maven' 
        jdk 'java'
  }
}
