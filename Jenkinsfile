pipeline{
    agent any

    stages{
        stage("build"){
            steps{
                echo 'building now!'
            }
        }
    }
        stages{
        stage("test"){
            steps{
                echo 'testing now!'
            }
        }
    }
        stages{
        stage("deploy"){
            steps{
                echo 'deploying now!'
            }
        }
    }
    post{
        always{
            emailext body: 'Summary' , subject: 'Pipeline Status', to: 'ishachoudhary521@gmail.com'
        }
    }
}