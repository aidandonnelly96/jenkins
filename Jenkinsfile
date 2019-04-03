pipeline {
  agent {
    docker {
      image 'python:3.5.1'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''sh \'echo "Hello World"\'
                sh \'\'\'
                    echo "Multiline shell steps works too"
                    ls -lah
                \'\'\''''
      }
    }
    stage('Test') {
      steps {
        sh 'echo \'Testing\''
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo \'Deploying\''
      }
    }
  }
}