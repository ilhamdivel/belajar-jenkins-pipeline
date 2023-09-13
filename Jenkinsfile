pipeline{
    agent any
    stages{
        stage("Build"){
            steps {
                echo("Hello Build");
            }
        }
        stage("Test"){
             steps {
                 echo("Hello Test");
             }
        }
        stage("Deploy"){
              steps {
                  echo("Hello Deploy");
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