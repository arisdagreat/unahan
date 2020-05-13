pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
            echo "puta"
            script {
			env.COMMIT = sh (
            script: 'cd $workspace && git rev-list HEAD | wc -l',
            returnStdout: true
           ).trim()
            echo ${env.COMMIT}
            }
        }
    }
}
