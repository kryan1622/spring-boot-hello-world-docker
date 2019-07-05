pipeline{
agent any
        stages{ 

                stage('---clean---'){
                        steps{
                                sh "mvn clean" -f /var/lib/jenkins/jobs 
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test" -f /var/lib/jenkins/jobs
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package" -f /var/lib/jenkins/jobs
                        }
                }
}
}
