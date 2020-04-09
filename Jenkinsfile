def workspace;
node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '2dde4745-523d-47d2-a139-82f8809c346a', url: 'https://github.com/VanshikaGupta24/HelloWorld.git']]])
        workspace = pwd()
    }
    stage('Static code Analysis')
    {
        echo "Static code Analysis"
    }
    stage('Build')
    {
        echo "Build the code"
    }
    stage('Unit testing')
    {
        echo "Unit testing"
    }
    stage('Delivery')
    {
        echo "Deliver the code"
    }
}
