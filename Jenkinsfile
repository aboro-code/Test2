pipeline {
    agent any
    tools{
        maven 'demo'
    }
    stages{
        stage('Checkout'){
            step{
                git url: 'https://github.com/aboro-code/Test2.git', branch: 'master'
            }
        }
        stage('Build'){
            steps{
                echo 'Building'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying'
            }
        }
    }
}