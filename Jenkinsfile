pipeline{
    tools{
        jdk 'JAVA_HOME1'
        maven 'M2_HOME1'
    }
    agent any
    stages{
        stage("checkout"){
            steps{
                git 'https://github.com/Pratik188/jenkinsrepo.git'
            }
        }
        stage("compile"){
            steps{
                sh 'mvn compile'
            }
        }
        stage("test"){
            steps{
                sh 'mvn test'
            }
        }
        stage("package"){
            steps{
                sh 'mvn package'
            }
        }
    }
}
