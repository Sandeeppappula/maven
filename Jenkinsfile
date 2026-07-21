@Library('mylibrary')_
node('built-in')
{
    stage('download')
    {
        cicd.gitdownload("maven")
    }
    stage('build')
    {
        cicd.gitbuild()
    }
    
}




