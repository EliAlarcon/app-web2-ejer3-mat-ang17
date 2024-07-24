node{
    stage('Revisión'){
        checkout scm
    }
    
    stage('Instalar dependencias'){
        bat 'npm install'
    }

    stage('Construir aplicación'){
        bat 'npm run ng build'
    }
}