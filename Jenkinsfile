pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
               echo "Srikanth pipeline checkout" 
            }
            //git checkout
        }
        stage('Build') {
            steps {
               echo "111 Srikanth pipeline Building" 
            }            
            //mvn clean package //this is for java code base
            //dotnet Build //this is for microsoft dotnet code base
            //npm build //this is for angular/react code base
        }
        stage('test') {
            //mvn test //junit
        }
        stage('scan') {
            //mvn verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=Srikanthm78_test345
            //mvn sonar:sonar //sonarcube credentials
            //service accounts
        }
        stage("Quality gate") {
            steps {
                //waitFprQualityGate abortPipeline: true
            }
        }
        stage('Artifactory') {
            //jFrog //url // credentials
        }
        stage('DeployToDev') {
        //connection to development server
        //publish -> CLI(AWS CLI, Azure CLI, Plugins)
        }
        stage('DeployToTest') {

        }
        stage('DeployToProd') {

        }
    }
}
