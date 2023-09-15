@Library('mylibrary')_

node('built-in')
{
    stage('Download_loans')
    {
      cicd.newDownload("maven.git")  
    }
    stage('Build_loans')
    {
      cicd.newBuild()
    }
    stage('Deploy_loans')
    {
      cicd.newDeploy("shared_library","172.31.1.73","testapp")
    }
}
