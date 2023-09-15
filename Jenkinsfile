@Library('mylibrary')_

node('built-in')
{
    stage('Download_master')
    {
      cicd.newDownload("maven.git")  
    }
    stage('Build_master')
    {
      cicd.newBuild()
    }
    stage('Download')
    {
      cicd.newDeploy("shared_library","172.31.1.73","testapp")
    }
}
