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
                
                git url: "https://github.com/venkatvaranasi8421/python-sample-cc",
                    credentialsId: 'SemVerPOC_2',
                    branch: main
                sh 'git add .'
                sh 'git tag -a ${next_version} -m "Your tag comment"'
                sh 'git commit -m "Updated tag and version'
                sh 'git push'
            }
        }
     
    }
}
