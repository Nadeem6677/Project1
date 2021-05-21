pipeline {
agent {
    dockerfile {
        filename 'Dockerfile'
        dir 'build'
        label 'test'
        args '-v /tmp:/tmp'
    }
}
}
