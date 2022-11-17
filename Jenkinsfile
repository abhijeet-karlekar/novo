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
        stage('The Message') { 
            steps {
                sh "echo Choice: ${params.ENVIRONMENT}"
                echo "Hey..This is Dev environment"
            }
        }
        
    }
}
