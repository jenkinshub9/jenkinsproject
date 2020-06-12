pipeline{
agent any
tools {
maven 'maven'
jdk 'jdk'
}
stages{
stage('clone repo'){
steps{
     
echo "clone the repository"
} }
stage('Test'){
steps{
echo "test the repository"
}  }
stage('Deploy')
{
steps{
echo "deploy the repository"
} }
}
post {
always {
echo "post the repository"
}   }  }
