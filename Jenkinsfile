pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'git@github.com:360CXservices/CICDTest.git', branch: 'DevelpoersBranch', credentialsId: 'Word-SSH')
        echo 'Build Completed'
      }
    }

    stage('build') {
      steps {
        build 'Virto-test'
        echo 'Build Completed'
      }
    }

    stage('Test') {
      steps {
        echo 'Test Completed'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment Completed'
      }
    }

  }
}