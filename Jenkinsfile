node {

    stage 'Checkout'
        checkout scm
    stage 'Build & UnitTest'   
        sh "docker-compose -f docker-compose.yml up --force-recreate" 
        sh "docker-compose -f docker-compose.yml down -v"
}
