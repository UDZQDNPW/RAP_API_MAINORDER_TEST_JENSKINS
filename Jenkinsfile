pipeline {
    agent any
    triggers {
        cron('H/15 * * * *')
    }
    stages {
        stage('Run E2E tests') {
            steps {
            bat 'npm -g install newman'    
            bat 'newman run Read.postman_collection.json --disable-unicode --suppress-exit-code 1'
            }
        }
    }
    
}

