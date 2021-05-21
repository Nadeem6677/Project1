pipeline {
    agent none
    stage ('Checkout') {
        agent any
        steps {
            git(
                url: 'https://github.com/Nadeem6677/Project1',
                credentialsId: 'test',
                branch: "master"
            )
        }
    }
    stage ('Build') {
        agent {
            dockerfile {
            filename 'Dockerfile'
        }
        steps {
            [...]
        }
}
    }
    [...]
}
