pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        dir(path: '/home/shiyanlou/Code') {
          git(credentialsId: '35a706cf-a65a-4a39-8f12-03547944ad6d', url: 'git@github.com:chang2358/test_git.git', branch: 'main')
        }

      }
    }

    stage('build') {
      steps {
        sh 'sudo -H pip install -r requirements.txt'
      }
    }

    stage('run') {
      steps {
        sh 'python app.py'
      }
    }

  }
}