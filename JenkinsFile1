pipeline{

    agent any


    tools{
        maven 'mymaven'
    }

    stages{
        stage('Clone the Repo'){
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        stage('Compile the code'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('Test the code'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Build the code'){
            steps{
                sh 'mvn package'
            }
        }
    }
}