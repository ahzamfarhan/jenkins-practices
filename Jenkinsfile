pipeline {
    agent any

    tools {
        maven 'Maven 3.8.1' // Replace with your Maven tool name
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
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
