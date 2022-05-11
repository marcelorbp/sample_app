#!/usr/bin/env groovy
pipeline {
    agent any

    tools {
        nodejs "NODE"
    }

    stages{
        stage('Checkout') {
            steps{
                git changelog: false, poll: false, url: 'https://github.com/renatasilva11/sample_app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'node test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy somewhere!'
            }
        }
    }
}
