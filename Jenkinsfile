pipeline{
    agent any

    stages{

        stage("build"){
            steps{
                timeout(time:1, unit:'MINUTES') {

                    sh 'mvn package'
                    // sh 'boxfuse run target/hello-1.0.war'
                }
        
            }
        }
    }

    post {
        failure {
            echo "Build Failed"
        }
    }
}