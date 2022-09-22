pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
  post{
    success {
     emailext attachLog: true, body: '', subject: 'failed', to: 'serge.kamgang@utrains.org' 
    }
  }
}
