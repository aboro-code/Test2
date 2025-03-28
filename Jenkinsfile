pipeline {
    agent any
    stages {
        stage('Checkout'){
            steps {
                git url: 'https://github.com/aboro-code/Test2.git' , branch: 'master'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps { // Add the steps block here
                echo 'Deploying...'
            }
        }
    }
}
