pipeline {
agent any
tools
{
 go 'install-Go1.14.5'

         }
environment {
GO111MODULES='on'

     }
stages{
    stage('build'){
      steps {

      sh  'go build'


}
}
stage('Test')
{

environment{
CODECOV_TOKEN = credentials('MY_SECRET')



}
steps
{
sh """
   go test ./... -coverprofile=coverage.txt
   curl -s https://codecov.io/bash | bash -s -
"""
}




}





    }























}
