pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name davidClusterEKS --template-body file://davidEKS.yml --region 'us-east-1'"
              }
		stage ('Update Stack') {
		steps {
		sh "aws cloudformation update-stack --stack-name davidClusterEKS --template-body file://davidNode.yml --region 'us-east-1'"
		}
	
		}	  
         }


     }
}
