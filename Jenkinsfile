pipeline {
    agent any
    tools{
        maven 'demo'
    }
    stages {
        stage('Checkout'){
            steps {
                git url: 'https://github.com/aboro-code/Test2.git', branch: 'master'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Run JAR') {
            steps { // Add the steps block here
                script{
                    def output = sh(script: 'java -jar target/simple-java-project-1.0-SNAPSHOT.jar', returnStdout: true)
                    echo "Output from the JAR: ${output}"
                }
            }
        }
    }
}