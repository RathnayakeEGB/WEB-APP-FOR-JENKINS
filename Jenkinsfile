pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
             bat   'mvn clean package'
             bat "docker build -t xxxx:${env.BUILD_ID} -f DockerFile ."
            }
        }
    }
}