#!/usr/bin/env groovy Jenkinsfile
pipeline {
    agent any
    stages {

        stage('Build'){
            if(isUnix()){
                sh 'gradle build --info'
            }
            else{
                bat 'gradle build --info'
            }
        }
        stage('Test'){
            if(isUnix()){
                sh 'gradle test --info'
            }
            else{
                bat 'gradle test --info'
            }
        }
    }
}

