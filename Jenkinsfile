pipeline {
    agent any
    stages {
        stage('myStage'){
            steps {
                sh 'ls -la' 
            }
        }
        stage('Build') {
            steps { 
                sh 'ls' 
            }
        }
        stage('Deploy') {
            steps { 
                sh 'echo  $HOME'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    cd $HOME
                    pwd
                    echo "Hello Siva"
                '''
            }
        }
    }
}
