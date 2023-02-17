pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG21CS830-1', wait: false
                 echo 'Build by PES1UG21CS830 successfully'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test by PES1UG21CS830 successfully'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by PES1UG21CS830 successfully'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
