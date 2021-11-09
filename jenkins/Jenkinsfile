pipeline {
  agent any
  environment {
    PATH = "/root/apache-maven-3.8.3/bin:${PATH}"
  }
  stages {
    stage("1st Stage") {
      steps{
        sh "hostname"
      }
    }
    stage("Build the project") {
      steps{
        sh "mvn clean package"
      }
    }
    stage("3rd Stage") {
      steps{
        sh "echo hello"
      }
    }
  }
}
