pipeline { 
agent any
    stages {
        stage('clone the repository') {
            steps {
                git 'https://github.com/khufia/jenkins-demo'
            }
        }
        stage('exec main') {
            steps {
		sh "chmod u+x main.py"
                sh "python3 main.py"
            }
        }
     stage('run tests') {
            steps {
		sh "chmod u+x test.py"
                sh "python3 test.py"
            }
        }
    } 
}
