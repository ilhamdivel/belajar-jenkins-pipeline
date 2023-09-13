pipeline{
    agent any
    stages{
        stage("Build"){
            steps {
             script {
                for ( int i = 0; i < 10; i++){
                    echo("Script  ${i}");
                }
             }

                echo("Start Build");
                bat("mvnw.cmd clean compile test-compile");
                echo("Finish Build");
            }
        }
        stage("Test"){
             steps {
                 echo("Start Test");
                 bat("mvnw.cmd test");
                 echo("Finish Test");
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