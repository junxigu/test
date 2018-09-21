pipeline {
  agent any
  stages {
    stage('steup') {
      parallel {
        stage('steup') {
          steps {
            git(url: 'https://github.com/junxigu/test.git', branch: 'master', changelog: true, credentialsId: 'junxigu')
          }
        }
        stage('setup') {
          steps {
            git(url: 'https://github.com/junxigu/test.git', branch: 'master', changelog: true, credentialsId: 'gujunxi')
          }
        }
      }
    }
    stage('') {
      steps {
        sleep 10
      }
    }
  }
}