pipeline{
	agent any
        stages{ 

                stage('---clean---'){
                        steps{
                                sh "mvn clean" -f /var/lib/jenkins/workspace/${JOB_NAME} 
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test" -f /var/lib/jenkins/workspace/${JOB_NAME}
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package" -f /var/lib/jenkins/workspace/${JOB_NAME}
                        }
                }
	}
}
