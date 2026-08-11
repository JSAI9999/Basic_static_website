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
            sh 'docker rmi -f static-website || true'
            sh 'docker build -t static-website .'
        }
    }

    stage('Docker Run'){
    steps {
         sh 'docker rm -f static_website || true'
        sh 'docker run -itd --name static_website -p 8089:80 static-website'

}
}

}
}
