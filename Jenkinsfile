pipeline{
    agent any
    environment{
        File_Name="JavaPipeline"
    }
    stages{
        stage('build'){
            steps{
                sh 'echo "Building..."'
                sh 'echo "${File_Name}"'
            }
        }
        stage('test'){
            steps{
                sh 'echo "Testing...'
            }
        }
        stage('deploy'){
            steps{
                sh 'echo "Deploying..."'
            }
        }
    }
}
post{
    always{
        echo "====++++always++++===="
    }
    success{
        echo "====++++only when successful++++===="
    }
    failure{
        echo "====++++only when failed++++===="
    }
}