#!/usr/bin/env groovy Jenkinsfile
Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    def gradleHome = tool 'Gradle4.7'
    env.PATH = "${gradleHome}/bin:${env.PATH}"
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

