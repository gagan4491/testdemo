pipeline {
    agent any 
    stages {

       stage('cloning from git') {
            steps {
            git branch: 'main', url: 'https://github.com/gagan4491/testtttt.git'

                //
            }
    }

 post {
    always {
      echo "I will always execute this!"
      cleanWs()
    }
  }
}
