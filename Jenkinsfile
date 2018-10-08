node {
  stage('scm checkout') {
    git 'https://github.com/pkeshab/springboot-jsp.git'
          }
  
  echo " Changing to another stage in the pipeline"
  
  stage('build the project')
    sh 'mvn clean package'
  
  #stage('archive the artifacts')
  # archiveArtifacts artifacts: '\'myfirstspring/*.zip\'', onlyIfSuccessful: true
  
  
  }



