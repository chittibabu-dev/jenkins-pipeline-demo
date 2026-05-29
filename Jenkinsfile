pipeline {

    agent any

    stages {

        stage('Checkout Validation') {
            steps {
                sh '''
                echo "===== CHECKOUT SUCCESS ====="

                pwd

                ls -la
                '''
            }
        }

        stage('Build') {
            steps {
                sh '''
                echo "===== BUILD ====="

                mkdir -p build

                echo "Application Build Successful" > build/build.txt

                cat build/build.txt
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                echo "===== TEST ====="

                echo "Tests Passed"
                '''
            }
        }

        stage('Deploy Simulation') {
            steps {
                sh '''
                echo "===== DEPLOY ====="

                hostname
                date

                echo "Deployment Simulation Completed"
                '''
            }
        }
    }
}
