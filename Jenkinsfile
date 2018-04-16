node {  
    stage('Checkout') {
      checkout scm
    }

    stage('Copy Docker-Compose') {
      sh 'scp Docker-Compose.yaml jenkins@mithras743:/home/jenkins'
    }
    
    stage('Docker-Compose') {
       sh 'ssh jenkins@mithras743 < docker-compose up -d'
    }
}
