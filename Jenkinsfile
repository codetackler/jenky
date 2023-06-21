pipeline {
  agent any
  triggers {
    fanin(upstreamProjects: "junky/master,jinky/master")
  }
  stages {
    stage('Jenky') {
      steps {
        sh '''
            echo "Aloha"
            sleep 10
        '''
      }
    }
  }
}
