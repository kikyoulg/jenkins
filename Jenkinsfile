pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh '''mvn clean package -Dmaven.test.skip=true
docker build -t registry.zet-fl.com/msmp/fedx-api:latest
docker push registry.zet-fl.com/msmp/fedx-api:${IMAGE_TAG}'''
          }
        }

        stage('sonar scan') {
          steps {
            sh 'echo "hello"'
          }
        }

      }
    }

    stage('push-image') {
      steps {
        sh 'docker push '
      }
    }

  }
}