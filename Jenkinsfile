pipeline {
  agent any
  options {
    buildDiscarder logRotator(numToKeepStr: '5'))
    disableConcurrentBuilds()
  }
  stages {
    stage('Hello') {
      steps {
        echo "hello"
      }
    }
  }
}
