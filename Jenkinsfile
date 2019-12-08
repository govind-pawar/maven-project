pipeline{
agent any
stages
{stage ('git clone')
{
steps
{git 'https://github.com/govind-pawar/maven-project.git'
}
}
}
{ stage ('compile code')
{ steps {
  withMaven(jdk: 'localjdk', maven: 'localmaven')
  { sh 'mvn compile'}}}
}
}
