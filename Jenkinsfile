#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building with EH edit...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing  with EH edit ...'
                sh 'npm test'
            }
        }
    }
}
