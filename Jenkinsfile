pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build'
        sh '/TestJenkins/helloWorld.sh'
      }
    }

    stage('Test') {
      steps {
        echo 'Test'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}