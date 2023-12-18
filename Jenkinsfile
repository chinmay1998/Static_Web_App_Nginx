pipeline{
    agent any
    stages{
        stage(ContinousDownload){
            steps{
                echo "Downloading the code from GitHub"
                git branch: 'master',url: 'https://github.com/chinmay1998/Static_Web_App_Nginx.git'
                echo "Downloading Completed"
            }
        }
        stage(ContinousDeployment){
            steps{
                echo "Deploying TheCode"
                sh 'sudo scp /var/lib/jenkins/workspace/Project1/* ubuntu@54.90.255.148:/var/www/html/'
                echo "Deployment Completed"
            }
        }
    }
}