pipeline {
  agent any
  stages {
   
    stage('Deploy ARM') {     
      steps {
        bat 'mvn deploy -P arm -Darm.target.name=local-4.4.0-ee -Danypoint.username=bdwivedi-Danypoint.password=Cisco@2022'
      }
    }
    stage('Deploy CloudHub') {
     
      steps {
        bat 'mvn deploy -P cloudhub -Dmule.version=4.4.0 -Danypoint.username=bdwivedi-Danypoint.password=Cisco@2022'
      }
    }
  }
}