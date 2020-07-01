pipeline {
  agent any
  stages {
    stage('Construir') {
      steps {
        sh 'echo Bienvenido a la descarga del codigo'

		sh 'rm -rf *'
		checkout scm
      }
    }

    stage('Unitarias') {
      steps {
        sh 'echo Unitarias'
      }
    }

    stage('Frontend') {
      steps {
        sh 'echo Front'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo deploy'
      }
    }

  }
}