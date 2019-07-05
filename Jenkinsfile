pipeline{
	agent any
        stages{ 

                stage('---clean---'){
                        steps{
                                sh "mvn clean -f /var/lib/jenkins/workspace/azurejenkins" 
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test -f /var/lib/jenkins/workspace/azurejenkins"
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package -f /var/lib/jenkins/workspace/azurejenkins"
                        }
                }
stage('--deploy--'){
                        steps{
                               sh "scp /var/lib/jenkins/workspace/azurejenkins/target/hello-world-0.0.1-SNAPSHOT.jar krystak@51.145.27.186:/home/krystak/"
                        }
                }
	}
}
