pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building a Dot Ner Core'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing a Dotnet  Core'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying Dot net Core'
      }
    }

  }
  environment {
    ChromeDriverPath = 'C:\\Driver\\Path\\ChromeDriver.exe'
  }
}