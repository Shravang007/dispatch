pipeline {
 agent {
 node { label 'workstation'}
 }

 stages {

 stage('Build') {
       steps {
       echo 'build with golang'
       }
  }
  stage('Unit Tests') {
        steps {
           echo 'Unit Tests'
        }
   }
   stage('Code Analysis') {
         steps {
            echo 'sonarqube'
          //sh 'sonar-scanner -Dsonar.host.url=http://172.31.93.52:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=dispatch'
         }
    }
    stage('Security Scans') {
          steps {
             echo 'Security Scans'
          }
     }
     stage('Publish a Artifact') {
           steps {
              echo 'Publish a Artifact'
           }
      }
 }
}