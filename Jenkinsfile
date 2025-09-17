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
    }
}