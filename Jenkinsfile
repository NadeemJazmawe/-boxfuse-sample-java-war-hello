pipeline{
    agent any

    stages{

        stage("build"){
            steps{
                
            sh 'mvn package'
            sh 'boxfuse run target/hello-1.0.war'
        
            }
        }



    }
}