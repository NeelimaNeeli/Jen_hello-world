pipeline{
  agent{
    label "slave1"
  }
  stages{
    stage("clone code form github"){
      steps{
        git 'https://github.com/NeelimaNeeli/Jen_hello-world.git'
      }
    }
  }
}
