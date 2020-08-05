pipeline {
    agent any 
    stages {
       stage('Prep') { 
            steps {
                sh 'echo "step 1"' 
            }
        }
       stage('Build') { 
            steps {
                sh 'env'
                sh 'echo "step 2"' 
            }
        }
        stage('Test') { 
            steps {
                sh 'set'
                sh 'ls -la'
                sh 'pwd'
                sh 'id'
                sh 'touch ./testing_file'
                sh 'chmod 777 ./testing_file'
                sh 'ls -l ./testing_file'
                sh 'echo ${BRANCH} - ${NEW_BRANCH}'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo "finito"'
            }
        }
    }
}
