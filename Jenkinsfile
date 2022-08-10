pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
    stage('Hello') {
      steps {
        echo "hello"
      }
    } 
    stage('cat README') {
      when{
	branch "fix-*"
     }
      steps {
        sh '''
	   cat REAME.md
	   '''
      }
    }
  }
<<<<<<< Updated upstream
=======
  post {
    always {
        junit(
          allowEmptyResults: true, 
          testResults: '**/build/test-results/test/*.xml'
        )
    }
  }
<<<<<<< Updated upstream
>>>>>>> Stashed changes
=======
>>>>>>> Stashed changes
}
