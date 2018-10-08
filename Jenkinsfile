node {
  stage('scm checkout') {
    git 'https://github.com/pkeshab/springboot-jsp.git'
          }
  
  echo " Changing to another stage in the pipeline"
  
  stage('build the project')
    sh 'mvn clean package'
  
  stage('archive the artifacts')
   
    archiveArtifacts '\'/var/jenkins_home/workspace/pipeline/target/hello-springboot-1.3.5.RELEASE.war\''
  }



