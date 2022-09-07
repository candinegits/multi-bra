Pipeline {
    agent any
    stages {
        stage('git-clone'){
            parallel{
                stage('paralel-1){
                    steps{
                        sh 'lscpu'
                    }
                }
                stage('parallel-1a){
                    steps{
                        sh'free -m'
                    }
                }
            }
        }
        stage('systemcheck-carine1'){
            parallel{
                stage('parallel-2'){
                    steps{
                        sh'free -g'
                    }
                }
                stage('parallel'-2a){
                    steps{
                        sh'lscpu'
                    }
                }
            }
        }
        stage('systemanalysis-stage'){
            parallel{
                stage('parallel-3'){
                    steps{
                        sh 'whoami'
                    }
                }
            }
        }
    }
}
