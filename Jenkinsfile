pipeline
{
    agent any
    stages
    {
        stage('clean')
        {
            steps
            {
                sh 'rm -rf *'
		    sh 'rm -rf /var/www/html/*'
                sh 'git clone https://gitlab.com/paragvyas236/demo.git -b master'    
            }   
        }

        stage('build')
        {
            steps
            {
              	sh 'cp -r demo/* /var/www/html/'
            }
        }
}

}