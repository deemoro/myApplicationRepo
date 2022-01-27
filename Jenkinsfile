pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
        sh 'MyWebApp/src/main/webapp/build.sh'
      }
    }

    stage('test') {
      steps {
        echo 'Testing'
        sh 'MyWebApp/src/main/webapp/test-all.sh'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
        sh 'MyWebApp/src/main/webapp/deploy.sh'
      }
    }

  }
}