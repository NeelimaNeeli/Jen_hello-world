pipeline{
  agent{
    label "test"
  }
  stages{
    stage("cloning the code"){
      steps{
        git credentialsId: 'neelima-GIT', url: 'https://github.com/NeelimaNeeli/Jen_hello-world.git'
      }
     
    }
  }
}
