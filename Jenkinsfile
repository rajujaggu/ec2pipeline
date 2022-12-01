pipeline{
    agent {label 'Docker'}
     stages {
        stage ('vcs')
        {
            steps{
              git url: 'https://github.com/rajujaggu/ec2pipeline.git',
                  branch: 'docker'
            }
        }
        stage ('docker1'){
            steps{
                sh 'docker info'
            }
        }
}

}