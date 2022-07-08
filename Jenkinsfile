pipeline {
    agent any 
    stages {
        stage('Hello Nashville') { 
            steps {
                echo "Today is sunny in Nashville"
                // 
            }
        }
        stage('AquaFina') { 
            steps {
                echo "water"
                // 
            }
        }
         stage('cloning from git') { 
            steps {
            git branch: 'main', url: 'https://github.com/gagan4491/testtttt.git'   
             
                // 
            }
        }
         stage('2cloning from git') { 
            steps {
                sh "git clone https://github.com/gagan4491/CI_CD.git"
        
    }
    }
        stage("display all the files") {
            steps {
                
               sh "ls "
               sh "pwd"
            }
        }
        stage("cleaning worksapce at the end "){
            steps{
                //  this stgae will beat the end always !!!!
                // cleanWs()
                echo "for not showing it error "
                
                sleep 30
            }
        }
}
 post {
    always {
      echo "I will always execute this!"
      cleanWs()
    }
  }
}
