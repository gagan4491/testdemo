pipeline {
    agent any 
    stages {
        stage('Hello Nashville') { 
            steps {
                echo "Today is sunny in Nashville from dev "
                // 
            }
        }
        stage('AquaFina') { 
            steps {
                echo " from dev "
                // 
            }
        }
         stage('cloning from git') { 
            steps {
            git branch: 'main', url: 'https://github.com/gagan4491/testtttt.git'   
             
                // 
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
                
            }
        }

        stage("doing docker stuff "){
            steps{
                sh "docker --version"
                sh "docker images"
                sh """
                    docker --version
                    docker images
                    docker ps
                    ls -la
                   """

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
