pipeline {
    agent any
    triggers {
        cron('H/15 * * * *')
    }
    stages {
        stage('Run E2E tests') {
            steps {
            bat 'run.bat'
            }
        }
    }
    
}

