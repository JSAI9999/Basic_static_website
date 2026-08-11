pipeline {

```
agent any

stages {

    stage('Clone') {
        steps {
            git branch: 'main',
                url: 'YOUR_GITHUB_REPOSITORY_UR'
        }
    }

    stage('Build Docker Image') {
        steps {
            sh 'docker build -t static-website:1.0 .'
        }
    }

}
```

}
