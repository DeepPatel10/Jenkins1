pipeline{

    agent any

    stages{

        stage("Build"){
            steps{
                withMaven(maven: 'maven_3_5_0)'){
                    sh 'mvn clean compile'
                }
            }
        }




        {

            steps {
                echo 'Building the application..'
            }
        }

        stage("Test"){
            steps{
                withMaven(maven: 'maven_3_5_0)'){
                    sh 'mvn test'
                }
            }
        }



        {

            steps{

                echo 'Testing The application..'
            }
        }

        stage("Deploy"){
            steps{
                withMaven(maven: 'maven_3_5_0)'){
                    sh 'mvn deploy'
                }
            }
        }




        {

           steps{

               echo "Deploying the Application.."
           }
        }
    }

}