node {
     def antVersion = 'AntDefault'
     withEnv( ["ANT_HOME=${tool antVersion}"] ) 
     stage('checkout source') 
     {
        // when running in multi-branch job, one must issue this command
        checkout scm
     }
     stage('Build') 
     {
        bat '%ANT_HOME%/bin/ant.bat fetchChanges'
     }
     
}
