node
{
  /*stage("fetch")
  {
    //git "https://github.com/G-Gowtham/java-automation"
    checkout scm
  }*/
  
  stage("test")
  {
    echo "hello testing git..."
    bat(/mvn package/)
  }
  stage('Results') 
  {
     junit '**/target/surefire-reports/TEST-*.xml'
     archiveArtifacts 'target/*.jar'
    }
}
