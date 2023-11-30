pipeline {
    agent any
    stages{
        stage("Clone Code"){
            steps{
                git branch: 'main',
                credentialsId: 'hamzeeee',
                url: 'https://github.com/Hamxaakhtar/django-notes-app.git'
            }
        }
    
        stage("Deploy"){
            steps{
                sh "docker-compose up --build -d"
            }
        }
    }
  }    
