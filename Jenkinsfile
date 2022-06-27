pipeline{
    agent any

    stages{

        stage("build"){
            sh 'mvn package'
            sh 'boxfuse run target/hello-1.0.war'
        }



    }
}