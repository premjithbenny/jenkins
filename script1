pipeline 
{
    agent any 
    stages 
    {
        stage(‘one’) 
        {
            steps
            {
                git branch: 'main', changelog: false, poll: false, url: 'https://github.com/premjithbenny/ci-cd.git'
            }
        }
        stage('two') 
        {
            steps
            {
                sh 'sudo apt install apache2 -y'
            }
        }
        stage(‘three’) 
        {
            steps
            {
                sh 'sudo cp -R . /var/www/html/'
            }
        }
        
        
    }
}
