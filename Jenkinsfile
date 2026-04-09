pipeline{
    agent any
    tool{
           maven 'Maven' 
    } 
 
    stages { 
        stage('Clone') { 
            steps { 
                git 'https://github.com/vijaykadam2405/maven_jenkins_demo.git' 
            } 
        } 
 
        stage('Build') { 
            steps { 
                bat 'mvn clean compile' 
            } 
        } 
 
        stage('Test') { 
            steps { 
                bat 'mvn test' 
            } 
        } 
 
        stage('Package') { 
            steps { 
                bat 'mvn package' 
            } 
        } 
    } 
}
