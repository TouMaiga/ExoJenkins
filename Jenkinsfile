pipeline {
   
    agent any
   
    stages {

        stage('get code from github + web hook pipeline') {
            steps {
                echo 'Pulling...';
                git branch: 'main',
                url : 'https://github.com/TouMaiga/ExoJenkins.git';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}