pipeline 
{
    agent any

    stages 
	{
        stage('Build') 
		{
            steps 
			{
                echo 'Build the Application'
            }
        }
		stage ('Test')
		{
			steps
			{
				echo 'Test the Application'
			}
		}
		stage('Deploy')
		{
			steps
			{
				echo 'Deploy the Application'
			}
		}
    }
    post
	{
		always
		{
		    emailext body: '''Hi Team,
look on this
Thanks,
Rafi D''', subject: 'Pipeline-status', to: 'rafid.atp1@gmail.com'	
		}
	}
}

	
