pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Bước này sẽ clone mã nguồn từ repository Git
                git 'https://github.com/yourusername/your-repo.git'
            }
        }
    }
    
    post {
        success {
            // Thực hiện các hành động sau khi pipeline chạy thành công
            echo 'Pipeline ran successfully!'
        }
        failure {
            // Thực hiện các hành động sau khi pipeline thất bại
            echo 'Pipeline failed!'
        }
    }
}
