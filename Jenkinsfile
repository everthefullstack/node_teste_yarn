pipeline {
    agent any

    stages {
        stage("run yarn build") {
            steps {
                echo 'executando yarn build'
                nodejs("Node-12.13.0") {
                    bat "yarn install"
                    bat "yarn build"
                    bat "yarn start"
                }
            }
        }
    }
}