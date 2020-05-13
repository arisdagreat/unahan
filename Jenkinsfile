pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
            echo "puta"
            script {
			env.COMMIT = sh (
            git rev-list HEAD | wc -l
            )
#           ).trim()
            echo ${env.COMMIT}
            }
        }
    }
}
