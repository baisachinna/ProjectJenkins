pipeline {
    agent {
        node {
            label 'MVN'
        }
    }
    options {
        skipStagesAfterUnstable()
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn verify'
            }
        }
        stage('JUnit Test'){
            steps{
                junit 'payslip/target/surefire-reports/*.xml'
            }
        }
    }
}