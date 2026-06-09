pipeline {
  agent any

  stages {

    stage('Checkout') {
      steps {
        git branch: 'main',
          url: 'https://github.com/sachingits/saucedemo-automation-framework.git'
      }
    }

    stage('Build & Test') {
      steps {
        bat 'mvn clean test'
      }
    }
  }
}