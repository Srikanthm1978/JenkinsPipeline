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
            steps {
               echo "111 Srikanth pipeline Testing" 
            }                        
            //mvn test //junit
        }
        stage('scan') {
            steps {
               echo "111 Srikanth pipeline Scanning" 
            }                        
            //mvn verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=Srikanthm78_test345
            //mvn sonar:sonar //sonarcube credentials
            //service accounts
        }
        stage("Quality gate") {
            steps {
                echo "111 Srikanth pipeline Quality Gate" 
                //waitFprQualityGate abortPipeline: true
            }
        }
        stage('Artifactory') {
            steps {
                echo "111 Srikanth pipeline Artifactory" 
                //waitFprQualityGate abortPipeline: true
            }            
            //jFrog //url // credentials
        }
        stage('DeployToDev') {
            steps {
                echo "111 Srikanth pipeline Dev" 
                //waitFprQualityGate abortPipeline: true
            }            
        //connection to development server
        //publish -> CLI(AWS CLI, Azure CLI, Plugins)
        }
        stage('DeployToTest') {
            steps {
                echo "111 Srikanth pipeline Test" 
                //waitFprQualityGate abortPipeline: true
            }            

        }
        stage('DeployToProd') {
            steps {
                echo "111 Srikanth pipeline PROD" 
                //waitFprQualityGate abortPipeline: true
            }

        }
    }
}
