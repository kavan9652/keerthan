pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "hello world"'
          }
        }

        stage('PRAPEL1') {
          steps {
            sh '''sleep 10
echo "prapel stage 1.1"'''
          }
        }

      }
    }

    stage('stage2') {
      parallel {
        stage('stage2') {
          steps {
            sh 'echo "stage 2"'
          }
        }

        stage('prapel2') {
          steps {
            sh '''sleep 10
echo "prapel pipeline 2.2"'''
          }
        }

      }
    }

  }
}