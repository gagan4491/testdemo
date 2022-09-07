pipeline {
    agent any 
    stages {

       stage('deploy') {
            steps {
            
            sh '''
            
            pwd
            ls 
          
             cp ../demo_master/target/springboot-helloworld.war /usr/share/tomcat/webapps/
             
             sleep 5
            '''

                //
            }
    }
    
    // stage("restarting tomcat "){
    //     steps{
              
                  

    //             sh './../../../../../usr/share/tomcat/bin/shutdown.sh'
            
    //       echo" shutting down the tomcat "
            
    //             sleep 60
              
    //       echo " starting up the  tomcat "
    //         sh './../../../../../usr/share/tomcat/bin/startup.sh'
    //             sleep 60             
    //         echo " applicaton should be ready "
        
            
    //     }
    // }
}
//  post {
//     always {
//       echo "cleaning Workspace!"
//       cleanWs()
//     }
//   }
}
