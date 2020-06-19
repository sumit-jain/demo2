pipeline {
    agent any

    environment {
        DEMO = '2'
    }

    stages {
        stage('stage1') {
            steps {
                echo "This is the build# $BUILD_NUMBER of demo $DEMO"
                sh '''
                    echo "Using multi line shell step"
                    chmod +x test.sh
                    ./test.sh
                '''
            }
        }
    }
}