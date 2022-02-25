pipeline {
    agent any
    environment { 
        next_version = nextVersion(writeVersion: true)
    }
    stages {
        stage ('Build') {
            steps {
              echo "Next Version of App:: ${next_version}"
            }
        }
     
    }
}
