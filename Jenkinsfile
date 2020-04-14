pipeline {
    agent any

    stages {
         stage ('compile code') {
             steps {
                sh 'mvn clean package'
             }
         }

         stage ('copy package') {
             steps  {
                 sh 'sudo cp target/SampleServlet.war /usr/share/tomcat/webapps'
             }
         }
        
        }
    }
  
