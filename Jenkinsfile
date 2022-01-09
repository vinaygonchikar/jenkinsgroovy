pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                echo 'buidlling the application'
             
            }
        }
    
        stage("test"){
            when {
                expression{
                    env.BRANCH_NAME == 'main'
                }
            }
            steps{
                echo 'testing the application' 
            }
        }
    
 
        stage("deploy"){
            steps{
                echo 'deploying  the application' 
            }
        }
    }
    post{
        succuss{
            echo 'succesfully executed'
        }
        failure{
            echo 'failed'
        }
        always{
            echo 'go and check '
        }
    }    
} 
