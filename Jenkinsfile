
pipeline {
  agent {
  label "new node"
}
stages {
    stage ('checkout') {
       steps {
        echo 'checkout scm'
        }
    }
    stage ('creation of the folder') {
       steps {
          sh 'cd /home/ubuntu; sudo mkdir avadutha4'
       }
    }
    stage ('creation of the folder on different server') {
      steps {
        label ('slave')
        
        sh 'cd /home/ubuntu; sudo mkdir rohith4'
        }
    }
}
}
