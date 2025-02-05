CODE_CHANGES = GETGITCHANGES()
pipeline{
  agent any
    stages{
      stage("build"){
         when{
           expression{
             BRANCH_NAME = 'main' && CODE_CHANGES == true
           }
         }
            steps{
              echo 'building the application'
               echo 'build2 the application'
               echo 'build3 the application'
            }
          }
       stage("test"){
         when{
           expression{
             BRANCH_NAME='main' || BRANCH_NAME='branch1'
           }
         }
            steps{
               echo 'testing the application'
            }
          }
       stage("deploy"){
            steps{
               echo 'deploying the application'
            }
          }
      }
}
