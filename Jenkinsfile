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
                sh 'scp -r /var/lib/jenkins/workspace/Project1/* ubuntu@54.221.16.179:/var/www/html/'
                echo "Deployment Completed"
            }
        }
    }
}
