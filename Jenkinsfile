pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''ls
pwd'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'echo "this is click pipeline"'
          }
        }

        stage('test2') {
          steps {
            echo 'my name is sharma'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy the code'
      }
    }

  }
}