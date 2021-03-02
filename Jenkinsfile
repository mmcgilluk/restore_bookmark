pipeline {
  agent any
  stages {
    stage('Create Dev Container') {
      steps {
        sshagent(credentials: ['mm_jkey']) {
          sh '''ssh -o StrictHostKeyChecking=no Mark@192.168.1.20 /Users/Mark/dxtoolkit2/dx_ctl_js_container --d delphixdemo -container_name \'Dev Container\' -action restore -timestamp \'Pristine Data\'
'''
        }

      }
    }

  }
}