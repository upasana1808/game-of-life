pipeline
{
    tools{
        jdk 'MyJDK'
        maven 'MyMaven'
    }
    agent none
    stages
    {
        stage('checkout')
        {
            agent any
            steps
            {
                git 'https://github.com/upasana1808/game-of-life.git'
            }
        }
        stage('compile')
        {
            agent any
            steps
            {
                bat 'mvn compile'
            }
        }
        stage('test')
        {
            agent any
            steps
            {
               bat 'mvn test'
            }
        }
        stage('package')
        {
            agent any
            steps
            {
                bat 'mvn package'
            }
        }
        
    }
    
    
}
