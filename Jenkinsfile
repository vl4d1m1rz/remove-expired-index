node('generic'){
    stage('checkout'){
        checkout scm
    }
    stage('clean elasticsearch'){
        sh 'chmod +x remove-expired-index.sh'
        sh './remove-expired-index.sh -e http://elasticsearch:9200'
    }
}
