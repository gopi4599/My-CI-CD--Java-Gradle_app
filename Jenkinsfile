pipeline{
    agent any 
    environment{
        VERSION = "${env.BUILD_ID}"
    }
    stages{
        stage("sonar quality check"){
            
            }
            steps{
                script{
                    withSonarQubeEnv(credentialsId: 'sonarpasswd') {
                            sh 'chmod +x gradlew'
                            sh './gradlew sonarqube --stacktrace'
                    }
                }
            }
        }
    }


