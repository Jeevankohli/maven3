@Library('mylibrary')_

node('built-in')
{
    stage('Download')
    {
      cicd.newDownload("maven.git")  
    }
    stage('Build')
    {
      cicd.newBuild()
    }
    stage('Download')
    {
      cicd.newDeploy("shared_librarywithscriptedpipeline","172.31.27.196","testapp")
    }
}
