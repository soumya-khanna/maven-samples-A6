pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/soumya-khanna/maven-samples.git', branch: 'master')
      }
    }
    stage('bisect') {
      steps {
        sh 'start 198644632661c67b6c32f59e9047c11a70685e15 98ac319c0cff47b4d39a1a7b61b4e195cfa231e5'
      }
    }
    stage('bisect') {
      steps {
        sh 'run mvn clean test'
      }
    }
  tools {
    maven 'SE465A6M'
    jdk 'SE465A6J'
  }
}
