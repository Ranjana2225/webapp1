pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
    stage('checkout'){
      steps{
        git 'https://github.com/Ranjana2225/webapp1.git'
      }
    }
    stage('compile'){
      steps{
        sh 'mvn compile'
      }
    }
    stage('test'){
      steps{
        sh 'mvn test'
      }
    }
    stage('deploy with ansible'){
      steps{
          sh 'ansible-playbook deploy.yml'
      }
      }
      }
      }
