pipeline{
 agent any
 stages{

stages('TEST'){
steps{
bat 'mvn test'
}
}
stage('Build'){
steps{
bat 'mvn install'
}
}
stage('Deploy'){
  steps{
bat 'mvn deploy'
}
}
}
}
