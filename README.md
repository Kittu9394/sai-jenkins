# sai-jenkins
pipeline{     agent any     stages{         stage('chekout'){             steps{                 checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/pubnub/java.git']])             }         }
