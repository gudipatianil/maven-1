pipeline{
    agent any
    tools{
        maven 'maven'
    }
    stages{
        stage('git init'){
            steps{
                git 'https://github.com/gudipatianil/maven-1.git'
            }
        }
        stage('compile'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('build'){
            steps{
                sh 'mvn package'
            }
        }
    }
}
