pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                echo "npm build"
                nodejs('Node-16.8.0'){
                    sh 'npm install'
                }
            }
        }
        stage("Run"){
            steps{
                echo "npm run"
                nodejs('Node-16.8.0'){
                    sh "node main.js"
                }
            }
        }
    }
}
