pipeline{
    agent any
     stages {
        stage ('vcs')
        {
            steps{
              git url: 'https://github.com/rajujaggu/ec2pipeline.git',
                  branch: 'main'
            }
        }
        stage ('ec2'){
            steps{
                sh """aws ec2 create-vpc --cidr-block 192.168.0.0/16 --region "us-west-2"
                      
                      
                
                
                """
            }
        }
}

}