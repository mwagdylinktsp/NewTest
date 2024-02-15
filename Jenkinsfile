pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/mwagdylinktsp/NewTest.git', branch: 'main')
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