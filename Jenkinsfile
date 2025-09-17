@Library('shared-library@main') _

import my_playground.example.Utils

pipeline {
    agent any

    stages {
        stage('Print Date') {
            steps {
                script {
                    def utils = new Utils(this)
                    utils.printDate()
                }
            }
        }
        stage('Clone'){
            steps {
                script {
                    def utils = new Utils(this)
                    utils.cloneRepo('https://github.com/rajiv1506/terraform.git')
                }
            }
        }
    }
}