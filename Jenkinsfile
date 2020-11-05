node('master') {
    stage('Pre Build') {
        echo 'Cleaning workspace'
        deleteDir()
    }

    stage('Checkout') {
        checkout scm
    }

    stage('Build') {
        bat 'mvn -B -DskipTests clean package'
    }

    stage('Test') {
        bat 'mvn test'
        junit 'target/surefire-reports/*.xml'
    }
}