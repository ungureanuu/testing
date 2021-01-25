pipeline{
    agent any
    stages {
        stage("Checkout availablity"){
            steps{
                sh "hostname"
                sh "echo 'welcome to steps in stage checkout'"
            }
        }
        stage("SCM-Clone"){
            steps{
                sh "date"
                sh "echo 'welcome to steps in stage steps'"
            }
        }
        stage("Build"){
            steps{
                sh "cal"
                sh "echo 'welcome to steps in stage Build'"
            }
        }
        stage("Test"){
            steps{
                sh "mvn --version"
                sh "echo 'welcome to steps in stage steps'"
            }
        }
    }
}
