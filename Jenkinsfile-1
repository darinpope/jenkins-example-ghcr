pipeline {
  agent any
  environment {
    GITHUB_TOKEN=credentials('github-token')
  }
  stages {
    stage('build image') {
      steps {
        sh 'docker build -t darinpope/jenkins-example-ghcr .'
      }
    }
  }
}