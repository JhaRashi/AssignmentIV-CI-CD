pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                git branch: 'develop', url: 'https://github.com/JhaRashi/AssignmentIV-CI-CD.git'
            }
        }
        stage('Build and Run Application') {
            steps {
                sh 'javac -d bin src/* JavaApplicationSum.java'
                sh'java -cp bin JavaApplicationSum'
            }
        }
    }
}
