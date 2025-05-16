@Library('jenkins-shared-lib') _   // This loads the shared library configured globally

import org.demo.Utils

def utils = new Utils(this)

pipeline {
    agent any

    stages {
        stage('Greet') {
            steps {
                sayHello('DevOps Ninja')  // from vars/
            }
        }

       stage('Class Call') {
            steps {
                script {
                    utils.printInfo("Running from aliased class instance.")
                }
            }
        }

        stage('Read Template') {
            steps {
                script {
                    def message = libraryResource('messages/welcome.txt')
                    echo message
                }
            }
        }
    }
}
