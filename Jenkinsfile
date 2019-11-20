pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git(url: 'https://github.com/bharathsem/simple-java-maven-app.git', branch: 'Master')
      }
    }

    stage('Test') {
      steps {
        bat 'mvn test'
      }
    }

    stage('Package') {
      steps {
        bat 'mvn package'
      }
    }

  }
}