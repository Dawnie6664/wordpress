pipeline {
    agent{
        label 'master'
    }
stages {

    stage ('Build Docker Image') {
        steps {
            sh ''' docker build -t wordpress:${BUILD_NUMBER} . '''
        }
    }
  }
}
