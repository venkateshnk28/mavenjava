pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage("Clone Code") {
            steps {
               git branch: "master", url: "https://github.com/venkateshnk28/javamaven.git"
            }
        }
        stage("Build Code") {
            steps {
                sh "mvn clean install"
            }
        }
     }
 }
