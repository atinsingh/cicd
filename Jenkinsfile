node {
    
    stage('Initialization') {
        sh 'echo dummy step'
        sh 'sleep 20'
    }

    stage('Testing'){
        parallel centos: {
            node('centos') {
                sh 'echo Hello from Centos'
                sh 'sleep 30'
            }
        },
        ubuntu: {
            sh 'echo Hello from Ubuntu'
            sh 'sleep 30'
        }
    }

    stage('Notify People') {
        sh 'echo Hello people'
    }
    stage('Notify 2') {
        sh 'echo Hello people'
    }


    stage('Notify 33') {
        sh 'echo Hello people'
    }

    //

}