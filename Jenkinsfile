pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning Repository...'
            }
        }

        stage('Build') {
            steps {
                sh '''
                echo "Building Java Project..."
                cd "Password Protection"
                mkdir -p build
                javac -d build src/*.java
                '''
            }
        }

        stage('Success') {
            steps {
                echo 'Build Successful!'
            }
        }
    }
}
