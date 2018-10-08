node {
  stage('scm checkout') {
    git 'https://github.com/pkeshab/maven-simple.git'
          }
  
  echo " Changing to another stage in the pipeline"
  
  stage('build the project')
    sh 'mvn clean package'
  }



