pipeline {
    agent any
    parameters {
        string(name: 'name', description: 'Please tell me your name?')
        string(address: 'address', description: 'enter your address')
        text(name: 'DESC', description: 'Describe about the job details')
        booleanParam(name: 'SKIP_TEST', description: 'Want to skip running Test cases?') 
        choice(name: 'BRANCH', choices: ['Master','Dev','test','stage'], description: 'Choose branch')
        password(name: 'SONAR_SERVER_PWD', description: 'Enter App password')
    }
    stages {
        stage('Printing Parameters') {
            steps {
                echo "Hello ${params.NAME}"
 
                echo "Job Details: ${params.DESC}"
 
                echo "Skip Running Test case ?: ${params.SKIP_TEST}"
 
                echo "Branch Choice: ${params.BRANCH}"
 
                echo "APP Password: ${params.SONAR_SERVER_PWD}"
            }
        }
    }
}
