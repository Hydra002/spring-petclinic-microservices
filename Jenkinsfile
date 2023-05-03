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
//         sh 'ls'
//         sh 'cd ./spring-petclinic-config-server'
//         sh 'pwd'
//         sh 'ls'
        dir('spring-petclinic-config-server'){
          sh '../mvnw spring-boot:run'
        }
      }
    }
  }
}
