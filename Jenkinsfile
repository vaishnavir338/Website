pipeline{
  agent any
  
    stages{
      stage("clone code"){
        steps{
          echo "cloning the code"
          git url: "https://github.com/vaishnavir338/Website.git", branch: "master"
        }
      }
      stage("Build"){
        steps{
          echo " Building the image"
          sh "docker build /var/lib/jenkins/workspace/pipeline -t Website"
        }
      }
    }
}
