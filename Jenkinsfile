pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn clean install -DskipTests'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_') {
                    sh 'mvn test'
                }
            }
        }


       
    }
}