pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the Git repository
                git branch: 'main', url: 'https://github.com/JhaRashi/AssignmentIV-CI-CD.git'
            }
        }
        stage('Build and Run Application') {
            steps {
                sh 'javac -d src/IV/JavaApplicationSum.java'
                sh'java -cp bin/IV/JavaApplicationSum JavaApplicationSum'
            }
        }
    }
}
