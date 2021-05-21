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
        }
      }
      steps {
          sh "echo completed"
      }
    }
  }
}
