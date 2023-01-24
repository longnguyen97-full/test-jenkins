pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                script {
                    // The below will clone your repo and will be checked out to master branch by default.
                    git credentialsId: 'test-jenkins-id', url: 'https://github.com/longnguyen97-full/test-jenkins.git'
                    // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
                    sh "ls -lart ./*"
                    // List all branches in your repo.
                    sh "git branch -a"
                    // Checkout to a specific branch in your repo.
                    sh "git checkout main"
                }
            }
        }
    }
}
