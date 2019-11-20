pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        bat 'mvn compile'
      }
    }

    stage('validate') {
      steps {
        bat 'mvn validate'
      }
    }

    stage('Clean Package') {
      steps {
        bat 'mvn clean package'
      }
    }

  }
}