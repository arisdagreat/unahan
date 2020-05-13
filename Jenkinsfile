pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
            echo "puta"
            script {
			env.COMMIT = sh (
            script: `git rev-list HEAD | wc -l`,
            returnStdout: true
           ).trim()
            }
            echo "${env.COMMIT}"
            echo "$workspace"

            script {
                        env.pwd = sh (
            script: 'pwd',
            returnStdout: true
           ).trim()
            }
            echo "${env.pwd}"



            }
        }
    }
}
