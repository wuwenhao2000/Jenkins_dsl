pipeline {
  agent any
  environment{
  NAME= "WENHAO"
  ROLE= "network engineer"}
  stages {
  stage('Build'){
      steps {
      sh 'echo "Build something"'
      sh 'pwd'
      sh 'ls -al'
      sh 'echo my name is $NAME and I am $ROLE ; exit 0'}
  post {
      always{echo "this will always run"}
      success{echo "this will run only success"}
      failure{echo "this will run only failure"}
      unstable{echo "this will run only unstable"}}}
  stage('Test'){
      steps {echo "Test something"}}}}