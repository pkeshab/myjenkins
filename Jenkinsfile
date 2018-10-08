node {
  stage('scm checkout') {
    git 'https://github.com/pkeshab/springboot-jsp.git'
          }
  
  echo " Changing to another stage in the pipeline"
  
  stage('build the project')
    sh 'mvn clean package'
  
  stage('upload the artifacts to nexus repo')
  {  
      def image = docker.image("jenkins/jenkins:lts")
    image.inside{ sh 'cp ${WORKSPACE}/target/*.war /opt}}
    sh 'ls /opt'             

   
    
  
 }
    



