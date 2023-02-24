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
        sh "chmod 777 /var/run/docker.sock"
        sh "docker pull tomcat"
      }
    }
  }
}
