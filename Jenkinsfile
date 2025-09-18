@Library('shared-library@main') _

import my_playground.example.Utils

pipeline {
    agent any

    stages {
        stage('Clone'){
            steps {
                script {
                    def utils = new Utils(this)
                    start_time = utils.printDate()
                    utils.cloneRepo('https://github.com/rajiv1506/java.git')
                }    
            }
        }
        stage('Test') {
            steps {
                script {
                    test.test()
                }
            }
        }
    }
}