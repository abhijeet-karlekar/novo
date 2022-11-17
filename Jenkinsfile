pipeline {
    agent {
    node {
        label 'zero'
        customWorkspace '/mnt/homeworkWS'
    }
}
    parameters {
  choice choices: ['Dev', 'QA', 'Stage', 'Test'], description: 'Pick any one', name: 'ENVIRONMENT'
    }
      stages {
        stage('Executing QA-Environment') { 
            steps {
                sh "echo Choice: ${params.ENVIRONMENT}"
                echo "Hey...this is QA"
            }
        }
        
    }
}
