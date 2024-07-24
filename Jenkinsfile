node{
    stage('Revisar'){
        checkout scm
    }
    
    stage('Instalar dependencias'){
        bat 'npm install'
    }

    stage('Construir aplicacion'){
        bat 'npm run ng build'
    }

    //Borrar carpeta del html
    stage('Limpiar carpeta destino'){
        bat 'rmdir C:\servidor\fire /s'
    }

    stage('Mover al servidor'){
        bat 'xcopy C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\angular-pipeline\\dist\\app-03\\browser  C:\\servidor\\fire /E /I /Y'
    }
}