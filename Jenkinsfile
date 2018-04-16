node {  
    stage('Checkout') {
      checkout scm
    }

    stage('Copy Docker-Compose') {
      sh 'scp docker-compose.yml jenkins@mithras743:/home/jenkins/agilion/'
    }
    
    stage('Docker-Compose') {
       sh 'ssh jenkins@mithras743 < docker-compose up -d'
    }
}
