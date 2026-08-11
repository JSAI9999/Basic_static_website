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
            sh 'docker build -t static-website2 .'
        }
    }

    stage('Docker Run'){
    steps {
        sh 'docker run -itd --name static_website -p 8089:80 static-website2'

}
}

}
}
