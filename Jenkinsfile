pipeline {
  agent any
   tools {
      maven 'SE465A6M'
      jdk 'SE465A6J'
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/soumya-khanna/maven-samples-A6.git', branch: 'master')
      }
    }

  }
}
