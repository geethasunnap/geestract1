pipeline {
  agent any
   stages {
    stage('compile stage') {
      steps {
        withMaven(maven: 'maven-3.5.4') {
        sh 'mvn clean compile'
        }
    }
   }
    stage('testing stage') {
      steps {
        withMaven(maven: 'maven-3.5.4') {
        sh 'mvn test'
        }
}
}
  stage('Install Stage') {
   steps {
    withMaven(maven: 'maven-3.5.4') {
    sh 'mvn install'
} 
}
}
}
}

