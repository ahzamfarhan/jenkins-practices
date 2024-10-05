pipeline {
    agent any

    // Add the 'tools' block here to specify the Maven version
    tools {
        maven 'Maven 3.8.1' // This should match the Maven installation name configured in Jenkins
    }

    stages {
        stage('Build') {
            steps {
                echo 'Firing Clean build Maven command that also includes test case execution...'
                sh 'mvn clean install'
            }
        }

        /*stage('Run') {
            steps {
                script {
                    // Kill any existing running instance of the application (optional)
                    sh 'pkill -f "java -jar target/sb-ecom-*.jar" || true'
                    
                    // Start the application
                    sh 'nohup java -jar target/sb-ecom-*.jar &'
                }
            }
        }*/
    }
}
