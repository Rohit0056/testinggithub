pipeline {
  agent any
  stages {
    stage('FETCHING CODE FROM GITHUB') {
      steps {
        git(url: 'https://github.com/Rohit0056/testinggithub.git', branch: 'master', poll: true)
      }
    }

    stage('Install APACHE2') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('DEPLYOMENT') {
      steps {
        sh 'sudo cp -R index.html /var/www/html/'
      }
    }

  }
}