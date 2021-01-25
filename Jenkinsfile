pipeline{
    agent any
    tools {
        maven 'maven1'
    }
    stages {
        stage("SCM"){
            steps{
                git changelog: false, url: 'https://github.com/ungureanuu/testing.git'
                echo ' First step to cennect to SourceCode'
            }
        }
        stage("Build code"){
            steps{
                sh label: '', script: 'mvn compile'
            }
        }
        stage("Test"){
            steps{
                sh "mvn --version"
                sh label: '', script: 'mvn test'
            }
        }
        stage("Publish Junit Report"){
            steps{
                junit '**/target/surefire-reports/*.xml'
            }
        }
    }
}
