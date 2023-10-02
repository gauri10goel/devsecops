pipeline {
  agent any

  stages {
      stage('Build Artifact  -  Maven') {
            steps {
              sh "mvn clean package -DskipTests=true"
              archive 'target/*.jar' 
            }
        } 
        
      stage('unit tests') {
            steps {
              sh "mvn test"
            }
        }       
    }
}
//hjbhdfhsvfh