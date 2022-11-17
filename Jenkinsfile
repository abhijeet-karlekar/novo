pipeline {
    agent {
    node {
        label 'zero'
        customWorkspace '/mnt/homeworkWS'
    }
}
    parameters {
  choice choices: ['Dev', 'Test', 'Stage', 'QA'], description: 'Pick any one', name: 'ENVIRONMENT'
    }
      stages {
        stage('The Message') { 
            steps {
                sh "echo Choice: ${params.ENVIRONMENT}"
                sh "echo Choice: ${params.ENVIRONMENT}"
            }
        }
        
    }
}
