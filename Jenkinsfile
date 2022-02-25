pipeline {
    agent any
    environment { 
        next_version = nextVersion()
    }
    stages {
        stage ('Build') {
            steps {
              echo "Next Version of App:: ${next_version}"
            }
        }
     
    }
}
