pipeline {
  agent any 
  stages {
    stage('One') {
      steps {
        echo 'Bienvenido al Pipeline'
      }
    }
    stage('Two') {
      steps {
        input('¿Desea continuar?')
      }
    }
    stage('Three') {
      when {
        not {
          branch "main"
        }
      }
      steps {
        echo "Hola Branch"
      }
    }
  }
}
