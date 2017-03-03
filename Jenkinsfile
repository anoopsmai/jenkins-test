pipeline {
  agent any
  stages {
    stage('fetch') {
      steps {
        git(url: 'https://github.com/anoopsmai/jenkins-test.git', poll: true)
      }
    }
    stage('build') {
      steps {
        sh 'echo "doing build"'
      }
    }
    stage('backup') {
      steps {
        sh 'echo "copying to s3"'
      }
    }
    stage('deploy') {
      steps {
        sh 'echo "call Ansible playbook here for deployment"'
      }
    }
  }
}
