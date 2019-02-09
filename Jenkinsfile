pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        sh '''$ echo \'#!/bin/sh\' > my-script.sh
$ echo \'echo Hello World\' >> my-script.sh
$ chmod 755 my-script.sh
$ ./my-script.sh'''
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}