pipeline {
  agent {
    node {
      label 'workstation'
    }
  }
  stages {
    stage('Docker build') {
     steps {
       sh 'docker build -t docker.io/tejaswinidockerhub/user .'
       }
     }
    stage('Docker Push') {
      steps {
        sh 'docker push docker.io/tejaswinidockerhub/user'
      }
    }
  }
}