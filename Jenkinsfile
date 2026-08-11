pipeline {

agent any

stages {

    stage('Clone') {
        steps {
            git branch: 'main',
                url: 'https://github.com/akramsyed8046/Basic_static_website.git'
        }
    }

    stage('Build Docker Image') {
        steps {
            sh 'docker build -t static-website:1.0 .'
        }
    }

}


}
