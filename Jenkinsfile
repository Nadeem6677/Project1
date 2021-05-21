pipeline {
    agent any
    stages {
    stage('Git checkout'){
      steps {
        git branch: 'master',
        credentialsId: 'test',
        url: 'https://github.com/Nadeem6677/Project1'
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
