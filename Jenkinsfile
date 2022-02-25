pipeline {
    agent any
    environment { 
        current_version = currentVersion()
        next_version = nextVersion(writeVersion: true)
    }
    stages {
        stage ('Build') {
            steps {
                echo "Current version of App:: ${current_version}"
              echo "Next Version of App:: ${next_version}"
            }
        }
     
    }
}
