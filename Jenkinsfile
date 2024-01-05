pipeline {
    agent any
    parameters {
        string(name: 'MYNAME', defaultValue: 'Mr Jenkins', description: 'Plz enter your name')
        string(name: 'MYSURNAME', defaultValue: 'Shaikh', description: 'Plz enter your surname')
        booleanParam(name: 'CHOICE', defaultValue: true, description: 'Plz provide choice')
    }
    stages {
        stage('Build') {
            steps {
                sh 'chmod +X ./name.sh'
                sh './name.sh ${params.MYNAME} ${params.MYSURNAME}'
            }
        }


    }
}
