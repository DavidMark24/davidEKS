pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name davidClusterEKS --template-body file://davidEKS.yml --region 'us-east-1'"
              }
         }


     }
}
