pipeline {
    agent any

    tools {
        maven 'Maven-3.9.11'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/phaniharika01/Repo1_maven.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Run Java App') {
            steps {
                sh 'java -cp target/maven-java-1.0-SNAPSHOT.jar com.example.App'
            }
        }
    }
}
