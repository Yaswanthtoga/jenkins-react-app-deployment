pipeline{
    agent none
     stages{
        stage('Run'){
            agent {
                docker { image 'node:16-alpine' }
            }

            steps{
                sh 'npm install'
                sh 'npm install -g create-vite'
                sh 'npm run dev'
            }
        }
     }
}