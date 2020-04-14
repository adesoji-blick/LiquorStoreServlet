pipeline {
    agent any

    stages {
         stage ('stage one') {
             steps {
                echo 'building package'
		sh 'mvn clean package'
             }
         }

         stage ('stage two') {
             steps  {
                 sh 'sudo cp target/SampleServlet.war /usr/share/tomcat/webapps'
		 echo 'successfuly deployed'
             }
         }
        
        }
    }
  
