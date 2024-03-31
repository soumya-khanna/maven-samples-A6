pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/soumya-khanna/maven-samples', branch: 'master')
      }
    }
    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }
    stage('test') {
      steps {
        sh 'mvn test'
      }
    }
    stage('verify') {
      steps {
        sh 'mvn verify'
      }
    }
    stage('clean') {
      steps {
        sh 'mvn clean'
      }
    }
  }
  tools {
    maven 'SE465A6M'
    jdk 'SE465A6J'
  }
}
