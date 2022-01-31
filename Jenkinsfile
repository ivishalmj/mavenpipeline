pipeline{
    agent any
    stages{
        stage('git clone'){
            steps{
                git branch: 'main', url: 'https://github.com/ivishalmj/mavenpipeline.git'
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn package'
            }
        }
        stage('deploy'){
            steps{
                echo "deployment successful"
            }
        }
    }
}
