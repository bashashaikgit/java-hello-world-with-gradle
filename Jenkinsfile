pipeline {
     agent any
     stages {
         stage('Clean Workspace') {
             steps {
                  deleteDir()                  
             }
         }
         stage('Clone Project') {
             steps {                  
                  checkout scm                  
             }
         }
         stage('Build') {
             steps {      
                  sh 'echo Debug'
                  sh 'pwd'
                  sh 'ls -lrt'
                  sh './gradlew clean build'
             }              
         }
     }
 }
