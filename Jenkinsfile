node
{
    stage("Github")
    {
  
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sunil9889/JenkinsHelloWorld.git']]])
    }
   stage("Hello World"){
      bat label: '', script: '''javac Hello.java
                java Hello'''
   }
}
