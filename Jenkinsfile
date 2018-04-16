#!/usr/bin/env groovy Jenkinsfile

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'gradle build --info'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }

    }
}
