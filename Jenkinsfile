pipeline{
     agent any
     parameters {
  choice choices: ['MYJavaApp', 'simple-node-js-react-npm-app'], name: 'repoName'
}

    stages{
        
        stage('checkout'){

            steps{
                sh '''
                env
                '''
                 env["$repoName"]
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'Mykey', url: 'https://github.com/harinipolina137/${env.repoName}']])

            
            }
        }
    }
}
