@Library('jenkins-shared-lib') _   // This loads the shared library configured globally

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                sayHello('Nani')  // Calls shared library function
            }
        }
    }
}
