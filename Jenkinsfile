def buildimage = docker.image('an4967/tizenrt:1.1');
pipeline {
    agent any
    stages {
        buildimage.pull();
        buildimage.inside("")
        {
            stage('Checkout Sources') {
                steps {
                    sh "echo abcd"
                }
            }
        }
    }
}