@Library('JenkinsLibs') _

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World from Git'
            }
        }

      stage('Medium') {
            steps {
                echo 'Medium World from Git'
            }
        }

      stage('Finish') {
            steps {
                echo 'Finish World from Git'
            }
        }

         stage('From shared lib') {
            steps {
                def x;
                first([name:'World', age:22])
                script{
                   x = first.calcul(6)
                }
                echo 'XXX:' x
            }
        }
    }
}
