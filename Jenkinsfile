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
        stage('Test1') {
            steps {
                echo 'Testing  with EH edit ...'
                sh 'npm test'
            }
        }
    
         stage('Test2') {
            steps {
                echo 'Testing 2 with EH edit ...'
                sh 'npm test'
            }
        }
           stage('Test3') {
            steps {
                echo 'Testing 3 with EH edit ...'
                sh 'npm test'
            }
        }
    
    }
}
