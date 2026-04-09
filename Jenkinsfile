pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'Hello World-Stage1 executed'
      }
    }

    stage('stage2') {
      steps {
        echo 'Hello World-stage2 executed'
      }
    }

    stage('parallel stage') {
      parallel {
        stage('parallel stage') {
          steps {
            echo 'stage3 executed'
            echo 'stage 3'
          }
        }

        stage('stage4') {
          steps {
            echo 'stage 4 executed'
          }
        }

      }
    }

  }
}