pipeline {
    agent any

    stages {
        //stage ('SCM Checkout'){
           // steps {
                   
                   //git 'https://github.com/TonyK11/time-tracker'
              //  git credentialsId: '9664629c-d13e-4c8c-9305-7e01ca0d2437', url: 'https://github.com/TonyK11/time-tracker/pom.xml'
           // }
       //}
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                //git 'https://github.com/TonyK11/time-tracker.git'
                //tool name: 'Maven 3.8.1', type: 'maven'
                // Run Maven on a Unix agent.
                sh 'mvn clean package'

                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }

            //post {
                // If Maven was able to run the tests, even if some of the test
                // failed, record the test results and archive the jar file.
                //success {
                  //  junit '**/target/surefire-reports/TEST-*.xml'
                  //  archiveArtifacts 'target/*.jar'
               // }
            //}
        }
    }
}
