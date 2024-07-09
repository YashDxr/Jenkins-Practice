pipeline{
    agent any
    environment{
        File_Name="JavaPipeline"
    }
    stages{
        stage('build'){
            steps{
                bat 'echo "Building..."'
                bat 'echo "$File_Name%"'
            }
        }
        stage('test'){
            steps{
                bat 'echo "Testing...'
            }
        }
        stage('deploy'){
            steps{
                bat 'echo "Deploying..."'
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
}
