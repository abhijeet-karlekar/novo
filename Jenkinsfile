pipeline {
    agent {
    node {
        label 'zero'
        customWorkspace '/mnt/homeworkWS'
    }
}
    parameters {
  choice choices: ['Dev', 'Test', 'Stage', 'QA'], description: 'Pick any one', name: 'Please, choose environment to run..'
    }
      stages {
        stage('The Message') { 
            steps {
                echo "Hey...This is Dev. environment"
            }
        }
        
    }
}
