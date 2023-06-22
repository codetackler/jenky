pipeline {
  agent any
  triggers {
    fanin(upstreamProjects: "junky/master,jinky/master", watchUpstreamRecursively: true)
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
