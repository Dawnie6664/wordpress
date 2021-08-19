pipeline {
    agent{
        label 'master'
    }
stages {

    stage ('Build Docker Image') {
        steps {
            sh ''' docker build -t wordpress:${GITHUB_BRANCH}-${BUILD_NUMBER} . '''
        }
    }
  }
}
