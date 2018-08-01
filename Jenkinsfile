node {
stage ('checkout')
{
checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'f4a41c19-e8de-47d4-a7a1-bc2ca3dadd0e', url: 'https://github.com/narrasubbarao/pipeline.git']]])
}
stage ('compile')
{
 echo "compile the code"
}
stage ('test')
{
echo "test the code"
}
stage ('package')
{
  echo "package the code"
}
stage ('install')
{
echo "install the code"
}
}
