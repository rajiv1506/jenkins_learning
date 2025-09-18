@Library('shared-library@main') _

import my_playground.example.Utils

pipeline {
    agent any

    stages {
        stage('Clone'){
            steps {
                script {
                    def utils = new Utils(this)
                    def start_time = utils.printDate()
                    utils.cloneRepo('https://github.com/rajiv1506/java.git')
                    def end_time = utils.printDate()
                    def time = end_time - start_time
                    echo "Time taken: ${time}ms"
                }
            }
        }
    }
}