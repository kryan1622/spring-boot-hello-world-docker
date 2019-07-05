pipeline{
	agent any
        stages{ 

                stage('---clean---'){
                        steps{
                                sh "mvn clean" -f /var/lib/jenkins/workspace/azurejenkins 
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test" -f /var/lib/jenkins/workspace/azurejenkins
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package" -f /var/lib/jenkins/workspace/azurejenkins
                        }
                }
	}
}
