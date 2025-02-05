
pipeline{
  agent any
    stages{
      stage("build"){
            steps{
              echo 'building the application'
               echo 'build2 the application'
               echo 'build3 the application'
            }
          }
       stage("test"){
         when{
           expression{
             BRANCH_NAME='deploy'
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
