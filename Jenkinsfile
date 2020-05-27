pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('1.1') {
      parallel {
        stage('1.1') {
          agent {
            node {
              label 'master'
            }

          }
          steps {
            sh 'echo hello'
          }
        }

        stage('2.1') {
          agent {
            node {
              label 'slave-1'
            }

          }
          steps {
            sh 'echo hello'
          }
        }

        stage('3.1') {
          agent {
            node {
              label 'slave-2'
            }

          }
          steps {
            sh 'echo hello'
          }
        }

      }
    }

  }
}