pipeline {
    agent any
    stages {
        stage('Checkout Sources') {
            sh "echo abcd"
        }
        def buildimage = docker.image('an4967/tizenrt:1.1');
        buildimage.pull();
        buildimage.inside("")
        {
            stage('Checkout Sources') {
                sh "echo abcd"
            }
        }
    }
}
