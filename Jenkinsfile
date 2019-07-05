pipeline{
	agent any
        stages{ 

                stage('---clean---'){
                        steps{
                                sh "mvn clean -f /var/lib/krystak/workspace/azurejenkins" 
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test -f /var/lib/krystak/workspace/azurejenkins"
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package -f /var/lib/krystak/workspace/azurejenkins"
                        }
                }
	}
}
