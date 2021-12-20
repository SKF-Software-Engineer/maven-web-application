node{
 
  /* Adding Maven home path*/
  
  def mavenHome = tool name:"maven3.8.4"
  
  /* Configuring GIT */
  
  stage('configuring git'){
    git branch: 'development', credentialsId: '544b6c33-3fbe-48b7-9de0-85c54121973f', url: 'https://github.com/SKF-Software-Engineer/maven-web-application.git' 
  }
  
  /* Configuring Maven */
  
  stage('configure maven build'){
    sh "${mavenHome}/bin/mvn clean package"
  }
}
