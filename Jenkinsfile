#!/usr/bin/env groovy
pipeline {
    agent any

    tools {
        nodejs "NODE"
    }

 node {

stage (‘Prepare environment’) {

git branch: ‘main’, url: ‘https://github.com/renatasilva11/sample_app.git’

sh ‘npm install’

}

stage (‘Code analyse’) {

sh ‘echo “Run some lints”’

}

stage (‘Unit test’) {

sh ‘echo “Tests will back”’

}

stage (‘Build’) {

sh ‘npm run clean’

sh ‘npm run build’

}
    
}
