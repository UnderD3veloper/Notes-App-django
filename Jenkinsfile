pipeline{
    agent any
    
    stages{
        stage("Code"){
            steps{
                echo "Cloning the code"
                git url:"https://github.com/UnderD3veloper/notes-app-django.git", branch: "main"
            }
        }
        
        stage("Build"){
            steps{
                echo "Building the image"
                sh "docker build -t note-app ."
            }
        }
        
        stage("Push to DockerHub"){
            steps{
                 echo "Pushing image to DockerHub"
            }
        }
        
        stage("Deploy"){
            steps{
                echo "Deploying the container"
            }
        }
        
    }
}

