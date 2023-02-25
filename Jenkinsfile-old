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
        sh "sudo chmod 777 /var/run/docker.sock"
        sh "docker pull tomcat"
      }
    }
    
    stage("removing old & building docker image"){
      steps{
        sh "docker stop tom"
        sh "docker rm tom"
        sh "docker rmi tommy"
        sh "docker build -t tommy /home/ubuntu/workspace/first/webapp/target"
      }
    }
    
    stage("deploying container"){
      steps{
        sh "docker run -d -p 8081:8080 --name tom tommy"
      }
    }
    
  }
}
