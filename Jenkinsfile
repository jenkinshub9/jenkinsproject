pipeline{
agent any
tools {
maven 'maven'
jdk 'jdk'
}
stages{
stage('clone repo'){
steps{
bat 'checkout scm'
bat 'mvn clean'
} }
stage('Test'){
steps{
bat 'mvn test   '
}  }
stage('Deploy')
{
steps{
bat 'mvn package  '
} }
}
post {
always {
junit '**/surefire-reports/*.xml'
}   }  }
