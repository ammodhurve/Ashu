pipeline {
        agent any

        stages {
            stage('Checkout') {
                 steps {
                         checkout scm
                       }}
                stage('Build') {
                  steps {
                         sh '/home/amrita/Documents/devops-tools/apache-tomcat-9.0.73/bin/mvn install'
                         }}
                stages('Deployment'){
                  steps {

                        sh 'cp target/Nykaa.war /home/amrita/Documents/devops-tools/apache-tomcat-9.0.73/webapps'
       }
}}}

