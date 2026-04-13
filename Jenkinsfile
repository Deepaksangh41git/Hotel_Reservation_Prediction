pipeline{
    agent any 

    stages{
        stage('Cloning Github repo to Jenkins '){
            steps{
                script{
                    echo 'Cloning Github repo to Jenkins ....... '
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-token1', url: 'https://github.com/Deepaksangh41git/Hotel_Reservation_Prediction.git']])
                }

            }
        }

        
    }
}