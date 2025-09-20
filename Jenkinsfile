pipeline{
    agent any
    stages{
        stage("Clone Repo"){
            steps{
                git branch: 'master', url: 'https://github.com/Edwinkorir38/java-todo.git'
            }
        }
        stage("Build Repo"){
            steps{
                sh "./gradlew clean build "
            }
        }
        stage("Test Code"){
            steps{
                sh "./gradlew test"
            }
        }
        
    }
}