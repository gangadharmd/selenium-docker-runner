pipeline{
  agent any
  stages {
    stage("Run Test"){
      steps{
        bat "docker-compose up --scale chrome=4"
      }
    }
    stage("Bring Grid Down"){
      steps{
        bat "docker-compose down"
      }

    }
  }
}