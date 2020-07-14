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


    }























}
