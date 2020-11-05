node('master') {
    stage('Pre Build') {
        echo 'Cleaning workspace'
        bat 'git clean -fdx'
    }

    stage('Checkout') {
        checkout(scm)
    }
}