pipeline {
    agent any
    environment {
        STAGING_ENV = "Staging"
        PRODUCTION_ENV = "Production"
    }
    stages {
        stage('Build') {
            steps {
                echo "Build the code using Maven"
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo "Run unit and integration tests using JUnit"
            }
        }
        stage('Code Analysis') {
            steps {
                echo "Analyse code quality using SonarQube"
            }
        }
        stage('Security Scan') {
            steps {
                echo "Scan for vulnerabilities using Snyk"
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo "Deploy the application to a staging environment using AWS EC2"
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo "Run integration tests in staging using Selenium"
            }
        }
        stage('Deploy to Production') {
            steps {
                echo "Deploy the application to the production environment using Ansible"
                echo "${PRODUCTION_ENV}: Deployment complete"
                echo "This is a test change to trigger polling"
                // check again 
            }
        }
    }
}
