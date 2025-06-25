pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building PipeLine-Test-Repo ...'
                // 例如对于Maven项目:
                // sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // 例如:
                // sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // 部署命令，如复制文件到服务器或构建Docker镜像
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed'
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
