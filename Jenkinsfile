@Library('jenkins-shared-library') _

pipeline{
    agent {
        label "ws"
    }
    stages{
        stage('Lint Checks'){
            steps{
                script{
                    sample.info("user")
                }
                sh "echo ***** Starting Style Checks ***** "
                sh "/home/centos/node_modules/jslint/bin/jslint.js server.js || true"
                sh "echo ***** Style Checks are completed ***** "

            }
        }
        stage('Static Code Analysis'){
            steps{
                sh "echo ***** Starting Static Code Analysis ***** "

            }
        }
    }
}