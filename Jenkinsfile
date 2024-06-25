pipeline {
    agent {
        node {
            label 'maven'
        }
    }
    
    parameters {
        string(name: 'person', defaultValue: 'Gourav patel')
        choice(choices: ['QA', 'PROD'], name: 'ENV')
    }
    
    stages {
        stage ('Hello'){
            input {
                message 'should we continue'
                ok 'okay'
            }
            steps {
                echo 'NAMASTE'
                echo "my env is: ${ENV}"
            }
        }
    }
}
