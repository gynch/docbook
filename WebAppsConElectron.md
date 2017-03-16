#Crear una webapp mediante NodeJS y Electron

## 1. configuración del entorno
- En primer lugar hay que instalar nodeJS de la web https://nodejs.org/es/download/
- Después de instalar la aplicación hay que crear un proyecto en el directorio en el que vayamos a crear la app
```
npm init
```
- Posteriormente instalamos electron 
```
npm install electron --save-dev
```
- Una vez instalado generamos un fichero javascript similar a éste. En este caso he creado una webapp de [Pomodoro Tracker](https://pomodoro-tracker.com/)

```
const electron = require('electron');
const {app, BrowserWindow, globalShortcut} = electron;

let mainWindow;

app.on('ready',() =>{
	mainWindow = new BrowserWindow({
		width:1000,
		height:700
	});
	mainWindow.setTitle('Pomodoro Tracker');
	mainWindow.loadURL('https://pomodoro-tracker.com/')
	
	mainWindow.on('closed',() =>{
			mainWindow = null;
	});
	
});


```

- Modificamos el fichero package.json que se encuentra en el directorio  que estemos generando la app de modo que en main esté el fichero js que hemos generado. En mi caso pomodorotracker.js
```
{
  "name": "pomodorotracker",
  "version": "1.0.0",
  "main": "pomodorotracker.js",
  "dependencies": {
    "electron": "^1.6.2"
  },
  "devDependencies": {
    "electron": "^1.6.2",
    "electron-packager": "^8.5.2"
  },
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC",
  "description": ""
}

```
- instalamos el paquete electron-packager
```
npm install electron-packager --save-dev
```
- Ejecutamos el siguiente script
```
node_modules\.bin\electron-packager pomodoroTracker.js . --platform=win32 --arch=ia64
```

* *Nota1*: Al instalar los ejecutables los guarda en node_modules\.bin
* *Nota2*: Genera una aplicación exe para Windows 64bits. Cambiando platform y arch se pueden obtener para otras arquitecturas
* *Nota3*: Para esta guía me he basado en este vídeo [Creando Whatsapp con electron] (https://youtu.be/2cFggyzThCc)






