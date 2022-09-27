pipeline {
  agent any
  stages {
    stage('build image') {
      parallel {
        stage('sonar scan') {
          steps {
            sh 'echo "hello"'
          }
        }

        stage('') {
          steps {
            sh 'echo "hello"'
          }
        }

      }
    }

    stage('push image') {
      steps {
        sh 'docker push '
      }
    }

    stage('pod update') {
      steps {
        sh 'echo "hello"'
      }
    }

    stage('metersphere') {
      steps {
        sh 'echo "hello"'
      }
    }

  }
}