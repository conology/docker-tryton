node {
    
    def customImage
        
    stage ('Checkout'){
        checkout scm
    }
    stage ('Build'){
        
        sh 'echo Deploying Env'
        sh 'docker-compose up -d --build'
    }/*
    stage ('Deploy') {
        
        sh 'echo Deploying Env'
        sh 'docker-compose up -d --build'
    }
    
    stage ('Configure') {
        sh 'docker run --link tryton-postgres:postgres -e DB_PASSWORD=password tryton/tryton trytond-admin -d tryton --all'
    }*/
}
