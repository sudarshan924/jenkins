pipeline(){
    agent any
    stages{
        stage('suda'){
            steps{
                sh 'ifconfig'
            }
        }
        stage('test'){
            steps{
                sh 'cat /etc/os-release'
            }
        }
        stage('depoly'){
            steps{
                sh 'df -h'
            }
        }
    }
}
