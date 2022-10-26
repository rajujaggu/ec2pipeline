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
                sh 'aws ec2 run-instances --image-id ami-0c09c7eb16d3e8e70 --count 1 --instance-type t2.micro --key-name tempkey --security-group-ids sg-0919be859cab53b7f'
            }
        }
}

}