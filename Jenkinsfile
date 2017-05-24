pipeline {
  agent any
  stages {
    stage('q') {
      steps {
        parallel(
          "q": {
            echo '123'
            
          },
          "svn": {
            svn(url: 'svn://172.24.118.105/CMO', changelog: true)
            
          }
        )
      }
    }
  }
  environment {
    qwwe = '123'
  }
}