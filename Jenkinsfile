pipeline{
    agent any
    stages{
        stage('git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/ivishalmj/mavenpipeline.git'
            }
        }
        stage('docker image'){
            steps{
                sh 'docker build -t myimage'
            }
        } 
    }
}
