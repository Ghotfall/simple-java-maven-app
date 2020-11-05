node('master') {
    stage('Pre Build') {
        echo 'Cleaning workspace'
        deleteDir()
    }

    stage('Checkout') {
        checkout(scm)
    }
}