pipeline{
    agent any
    stages{
        stage("Hello"){
            steps {
                echo("Hello Pipeline");
            }
        }
    }
    post {
        always{
            echo "Always Say Hello";
        }
         success {
            echo "Yey Success";
         }
         failure {
            echo "Oh no, Failure";
         }
         cleanup {
            echo "Dont care, success or no";
         }
    }
}