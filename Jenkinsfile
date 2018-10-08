node {
  stage('scm checkout') {
    git 'https://github.com/pkeshab/springboot-jsp.git'
          }
  
  echo " Changing to another stage in the pipeline"
  
  stage('build the project')
    sh 'mvn clean package'
  
  stage('upload the artifacts to nexus repo')
  
nexusPublisher nexusInstanceId: '1123', nexusRepositoryId: 'myfirstapplicationnexus', packages: [[$class: 'MavenPackage', mavenAssetList: [[classifier: '', extension: '', filePath: '/var/jenkins_home/workspace/pipeline/target/*.war']], mavenCoordinate: [artifactId: 'hello-springboot', groupId: 'org.springframework.boot', packaging: 'war', version: '1.3.5.RELEASE']]]  
 }
    



