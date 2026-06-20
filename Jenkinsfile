pipeline {
    agent any
    tools { nodejs 'node-22' }
    stages {
        stage('Install') { steps { sh 'npm ci' } }
        stage('Type Check') { steps { sh 'npm run typecheck' } }
        stage('Lint') { steps { sh 'npm run lint' } }
        stage('Test') { steps { sh 'npm test' } }
        stage('Build') { steps { sh 'npm run build' } }
    }
}
