pipeline{
    agent {
        docker{
            image 'ruby'
        }
    }
    
    stages{
        stage('Build'){
            steps{
                echo 'Building or Resolve Dependencies!'
                sh 'bundle install'
            }
        }
        stage('Tests'){
            steps{
                echo 'Running regression tests'
            }
        }
        stage('UAT'){
            steps{
                echo 'Wait for User Acceptance'
                input(message: 'Go to production?', ok: 'Yes' )
            }
        }
        stage('Prod'){
            steps{
                echo 'WebApp is Ready :)'
            }
        }
    }
}