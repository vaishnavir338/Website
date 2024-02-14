pipeline{
  agent any
  
    stages{
      stage("clone code"){
        steps{
          echo "cloning the code"
          git url: "https://github.com/vaishnavir338/Website.git", branch: "master"
        }
      }
      stage('Building image') {
        steps{
          echo "Building image"
          sh "docker build -t website ."
        }
      }
      stage('deploy on dockerhub') {
        steps{
          echo "deploy on dockerhub"          
        }
      }
      stage("Deploy"){
        steps{
          echo"Deploying the container"         
        }
      }
        }
      }      
  
