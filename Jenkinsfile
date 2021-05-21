pipeline {
    agent none
    stages {
    stage('regularStage'){
      steps{
        sh 'time'
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
