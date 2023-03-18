pipeline{
     agent any
    stages{

        stage('checkout'){

            steps{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'Mykey', url: 'https://github.com/harinipolina137/MYJavaApp']])
            }
        }
    }
}