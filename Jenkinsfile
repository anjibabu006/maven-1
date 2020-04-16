node('master')
{
    stage('ContinuousDownload') 
    {
         git 'https://github.com/selenium-saikrishna/maven.git'
    }
    stage('ContinuousBuild') 
    {
         sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment')
    {
        sh label: '', script: 'echo "Deployment completed" '
    }
    stage('ContinuousTesting')
    {
        //git 'https://github.com/selenium-saikrishna/FunctionalTesting.git'
        sh label: '', script: 'echo "Testing completed" '
    }
     stage('ContinuousDelivery')
    {
        //input message: 'Waiting for Approval from the DM', submitter: 'Srinivas'
        sh label: '', script: 'echo "Continious delivery completed" '
    }
    
    
}

