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

    stage('Mover al servidor'){
        bat 'xcopy C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\angular-pipeline\\dist\\app-03\\browser  C:\\servidor\\fire /E'
    }
}