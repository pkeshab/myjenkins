node {
  stage('scm checkout') {
    git 'https://github.com/pkeshab/springboot-jsp.git'
          }
  
  echo " Changing to another stage in the pipeline"
  
  stage('build the project')
    sh 'mvn clean package'
  
  stage('archive the artifacts')
   def image = docker.image("sonatype/nexus3")
    image.inside { 
     sh "cp ${WORKSPACE}/pipeline/target/*.war /opt"
 }
    
  }



