pipeline {
  agent any
  stages {
    stage('Construir') {
      steps {
        sh 'echo Bienvenido a la descarga del codigo'

		sh 'rm -rf *'
		checkout scm
		
		sh 'echo Limpiar  Maven'
		sh 'mvn clean'
		
		sh 'echo Compilar  Maven'
		sh 'mvn compile'
		
		sh 'echo Empaquetar Maven'
		sh 'mvn package'
		
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