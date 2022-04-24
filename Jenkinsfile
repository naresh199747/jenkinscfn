pipeline {
    agent any
    stages{
        stage('clone repo')  {
            steps  {
          sh "export AWS_DEFAULT_REGION=us-east-1"
          sh "aws cloudformation create-stack --stack-name mytemaplate --template-body file://cftemplate.json --region 'us-east-1'"
            
            }
        } 
    }
}
