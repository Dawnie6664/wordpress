pipeline {
    agent{
        label 'master'
    }
stages {

    stage ('Build Docker Image') {
        when {
            anyOf {branch 'main'; branch 'master'} 
        }
        steps {
            sh ''' docker build -t wordpress:${GITHUB_BRANCH}-${BUILD_NUMBER} . '''
        }
    }
  }
}
