pipeline {
    agent any
    parameters {
        string(name: 'Branch', defaultValue: 'default', description: 'select which branch you want to select')
        booleanParam(name: 'Rebuild_Database' , defaultValue: true, description: 'Should we rebuild the database.')
        booleanParam(name: 'Deploy' , defaultValue: true, description: 'Should we Deploy the application')
        choice(name: 'Environment' , choices: 'Integration', description: 'used for posgress.sh and code deployment')
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.Branch}"
                echo "Hello ${params.Rebuild_Database}"
                echo "Hello ${params.Deploy}"
                echo "Hello ${params.Environment}"
            }
        }
    }
}
