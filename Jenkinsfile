pipeline {
  agent any
  stages {
    stage('Checkout Scm') {
      steps {
        git(url: 'https://innersource.accenture.com/scm/~r.k.srivastava/sdo2-ide.git', credentialsId: 'GIT_IDE')
      }
    }

    stage('No Converter-0') {
      steps {
        echo 'No converter for Builder: hudson.plugins.gradle.Gradle'
      }
    }

  }
  post {
    always {
      echo 'No converter for Publisher: hudson.plugins.git.GitPublisher'
    }

  }
  options {
    buildDiscarder(logRotator(daysToKeepStr: '2', numToKeepStr: '2'))
  }
}
