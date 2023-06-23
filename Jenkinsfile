pipeline {
  agent any
  triggers {
    fanin(upstreamProjects: "junky/master,jinky/master", watchUpstreamRecursively: true)
  }
  parameters {
    extendedChoice(
      name: 'HOST_PLATFORMS',
      type: 'PT_MULTI_SELECT',
      value: 'debiam_amd64,debian_arm64,debian_i386,debian_armv7hf',
      defaultValue: 'release'
    )
    choice(name: 'BUILD_MODE', choices: ['release','debug'])
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
