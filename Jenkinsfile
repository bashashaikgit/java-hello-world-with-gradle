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
                  bat 'echo Debug'
                  bat 'pwd'
                  bat 'ls -lrt'
                  bat './gradlew clean build'
             }              
         }
     }
 }
