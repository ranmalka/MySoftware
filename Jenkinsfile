properties([pipelineTriggers([pollSCM('*/30 * * * *')])])
pipeline {
    agent any

    stages {
        stage('git') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
