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
                sh 'scp /var/lib/jenkins/workspace/project2/'
                echo "Deployment Completed"
            }
        }
    }
}