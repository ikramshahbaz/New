pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '/var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/maven/bin/mvn clean'
      }
    }

    stage('Test') {
      steps {
        sh '/var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/maven/bin/mvn test'
      }
    }

    stage('Deploy') {
      steps {
        sh '/var/jenkins_home/tools/hudson.tasks.Maven_MavenInstallation/maven/bin/mvn package'
      }
    }

  }
}
