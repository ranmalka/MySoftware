properties([pipelineTriggers([pollSCM('*/30 * * * *')])])
pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                sh 'python3 main.py'
            }
        stage('click') {
            steps {
                sh 'python3 click.py'
            }
        stage('welcome') {
            steps {
                sh 'python3 welcome.py'
            }
        }
    }
}
