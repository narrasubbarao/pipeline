node {
stage ('checkout')
{
checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'f4a41c19-e8de-47d4-a7a1-bc2ca3dadd0e', url: 'https://github.com/narrasubbarao/pipeline.git']]])
}
stage ('compile')
{
  mvnHome = tool 'apache-maven-3.5.0'
sh 'mvn compile'
}
stage ('test')
{
sh 'mvn test'
}
stage ('package')
{
sh 'mvn package'
}
stage ('install')
{
sh 'mvn install'
}
}
