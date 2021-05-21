pipeline {
    agent any
    stages {
    stage('regularStage'){
      steps{
        sh "echo hey"
      }
    }
    stage('dockerStage') {
      agent {
        dockerfile {
          filename 'Dockerfile'
          dir 'test'
          label 'Test'
        }
      }
      steps {
          sh "echo completed"
      }
    }
  }
}
