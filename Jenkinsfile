pipeline
{
    agent any
    stages
    {
        stage('Compile')
        {
            steps
            {
                dir('src')
                {
                    bat 'javac hi.java'
                }
            }
        }
        stage('Run')
        {
            steps
            {
                dir('src')
                {
                    bat 'java hi'
                }
            }
        }
    }
    post
    {
        success
        {
            echo 'BUILD SUCCESSFUL'
        }
        failure
        {
            echo 'BUILDFAILED'
        }
    }
}