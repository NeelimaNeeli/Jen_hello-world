pipeline{
  agent{
    label "test"
  }
  stages{
    stage("cloning the code"){
      steps{
        git  'https://github.com/NeelimaNeeli/Jen_hello-world.git'
      }
     
    }
    
    stage("building the code"){
      steps{
        sh "mvn clean install"
      }
    }
    
    stage("downloading tomcat docker image"){
      steps{
        sh "docker pull tomcat"
      }
    }
  }
}
