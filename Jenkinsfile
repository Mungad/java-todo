pipeline{
    agent any
    stages {
        stage("Clone repo"){
            steps{
                git url:'https://github.com/Mungad/java-todo.git', branch:"master"
            }
        }
        stage("Build Repo"){
            steps{
                sh "./gradlew build"
            }
        }
        stage("Test Repo"){
            steps{
                sh "./gradlew test"
            }
        }
    }
}