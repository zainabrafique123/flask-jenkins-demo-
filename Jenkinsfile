pipeline {
    agent any
    stages {
        stage('Build & Run Flask') {
            steps {
                bat '''
                echo "Building Flask App"
                python -m venv venv
                call venv\\Scripts\\activate.bat
                python -m pip install --upgrade pip
                pip install -r requirements.txt
                python app.py
                '''
            }
        }
    }
}
