pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        dir(path: '/home/shiyanlou/Code') {
          git(url: 'git@github.com:chang2358/test_git.git', branch: 'main', credentialsId: 'd5851f34-fb2e-47be-b510-17a380d5279d')
        }

      }
    }

  }
}