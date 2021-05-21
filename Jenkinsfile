pipeline {
    agent none
    stages {
    stage('regularStage'){
      steps{
        sh 'some shell command to run on the node'
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
          sh 'date'
      }
    }
  }
}
