#!/usr/bin/env groovy
pipeline {
    agent any

    tools {
        nodejs "NODE"
    }

 node {

stage  {

git branch: ‘main’, url: ‘https://github.com/renatasilva11/sample_app.git’

sh ‘npm install’

}

stage  {

sh ‘echo “Run some lints”’

}

stage  {

sh ‘echo “Tests will back”’

}

stage  {

sh ‘npm run clean’

sh ‘npm run build’

}
    
}
}
