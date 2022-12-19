pipeline {
    agent {label 'docker'}
    stages {
        stage ('src') {
            steps{
                git url:"https://github.com/gowthamlearning/saleor-core.git",
                    branch:"main"
            }
        }
        stage('build image') {
            steps{
            sh """ docker image build -t gowthi1404/saleor-core:dev-19122022 .
               docker image push gowthi1404/saleor-core:dev-19122022 """ }
        }
    }
}