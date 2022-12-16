node
{
  def mavenHome = tool name: "maven3.8.6"
  
  stage("CheckoutCode")
  {
   git credentialsId: '2472694e-e5cf-4630-b5db-14653050e0cd', url: 'https://github.com/007harish0512/maven-web-application.git'
  }
   stage("Build")
  {
   sh "${mavenHome}/bin/mvn clean package"
  }    
  /*
  stage ("ExecutesonarqubeReport")
   {
   sh "{mavenHome}/bin/mvn sonar:sonar"
   }
   stage("uploadartifactintonexus")
   {
   sh "${mavenHome}/bin/mvn deploy"
    }
    */
}
