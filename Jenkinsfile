def workspace;
node
{
    stage ('Checkout SCM'){
    
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'c8e73172-f8de-47b1-9064-b7d4fa206d2d', url: 'https://github.com/yreddyp/jenkinsint.git']]])
    workspace =pwd()    
        
    }
    
    stage('validate')
    {
        echo " validate the code"
    }
    
    stage('compile')
    {
        echo " Compile the code"
    }
        
}
