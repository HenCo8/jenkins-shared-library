# Jenkins Shared Library

A simple Jenkins Shared Library for practicing reusable pipeline steps.

## Usage

```groovy
@Library('myLibrary') _

pipeline {
    agent any

    stages {
        stage('Test Shared Library') {
            steps {
                helloWorld('Jenkins Students')
            }
        }
    }
}
