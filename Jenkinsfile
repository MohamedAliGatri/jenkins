pipeline{
    agent any
    tools{
        maven "MAVEN"
    }
    stages{
        stage("Git checkOut"){
            steps{
                echo "TESTING WEBHOOKS WITH NGROK again"
            }
        }
        stage("Maven compile"){
            steps{
                echo "compile maven"
                sh 'mvn package'
            }
        }
        stage("SonarTest integration"){
            steps{                
                sh "mvn sonar:sonar"
            }
        }
    }
    
}
