pipeline {
  agent any
  stages {
    stage('Fetching Source Code') {
      steps {
        git 'https://github.com/Hydra002/spring-petclinic-microservices.git'
      }
    }
    stage('Starting Config Server') {
      steps {
        sh script 'cd spring-petclinic-config-server'
        sh script '../mvnw spring-boot:run'
      }
    }
  }
}
