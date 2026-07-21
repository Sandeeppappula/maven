@Library('mylibrary')_
node('built-in')
{
    stage('download_master')
    {
        cicd.gitdownload("maven")
    }
    stage('build_master')
    {
        cicd.gitbuild()
    }
    stage('deploy_master')
    {
        cicd.gitdeploy("172.31.8.161","testapp1")
    }
    stage("testing_master")
    {
        cicd.gittesting("FunctionalTesting")
    }
    stage("delivery_master")
    {
        cicd.gitdelivery("172.31.3.43","prodapp2")
    }
}




