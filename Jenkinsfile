pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'dev'
      }
    }

    stage('build') {
      steps {
        echo 'build'
      }
    }

    stage('test') {
      steps {
        echo 'test'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'uat'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'operate'
          }
        }

      }
    }

  }
}