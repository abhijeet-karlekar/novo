pipeline {
    agent {
    node {
        label 'zero'
        customWorkspace '/mnt/homeworkWS'
    }
}
    parameters {
  choice choices: ['Dev', 'Test', 'Stage', 'QA'], description: 'Pick any one', name: 'Choose'
    }
      stages {
        stage('The Message') { 
            steps {
                sh "echo Choice: ${params.Choose}"
                echo "Hey...This is Dev. environment"
            }
        }
        
    }
}
